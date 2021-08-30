# Flip动画

F：First
l：Last
i：invert
p：play

Flip是一种动画思路，针对列表动画过渡

具体过程如下

1. First：记录每个元素的起始坐标
2. Last：计算每个元素的结束坐标
3. Invert：将元素平移到原来的位置
4. Play：应用动画、平移

<!-- 伪代码 -->
```javascript

// 1. First
record(container)
// 改变元素位置
change();

// 2：last => 3：invert => 4：play
move(container); // 让元素真正实现移动
```
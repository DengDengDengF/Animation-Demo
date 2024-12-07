[TOC]



### 3次贝塞尔动画

```js
/* 
 t 参数，取值范围为[0,1]
 p0   起点的(x/y)
 p1   控制点1的(x/y)
 p2   控制点2的(x/y)
 p3   终点的(x/y)
 B(t) t点的(x/y)
*/
B(t)=(1-t)^3 * p0 + 3 * (1-t)^2*p1 + 3*(1-t)^2*p2 + t^3 * p3;
然后逐帧画出来sss
```

### svg路径动画

```js
stroke-dasharray: 20;//实线20 空白20 实线20 空白20 .。。。。。
strok-dashoffset:相对于绘制的起点偏移的量，正(左偏) 负(右偏)

过程：
//隐藏
dom.style.strokeDasharray = dom.getTotalLength();
dom.style.strokeDashoffset = dom.getTotalLength();

然后使用 requestAnimationFrame逐帧减少 dom.style.strokeDashoffset 的大小
```

### 3.canvas拖拽

```
略ffffffffffffffff
```


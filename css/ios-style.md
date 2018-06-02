1. ios中惯性滑动
```
  (1) overflow: auto可以滑动但没有惯性效果
  (2) 要有惯性效果需加上：-webkit-overflow-scrolling: touch
  (3) 当所在元素有position:relative或absolute或fixed时，滚动会有“假死”现象
      即上一次停下来后，下一次继续滚动前有几秒钟不响应
  (4) 解决办法是加一个z-index:1
```

2. ios中多级嵌套flex布局
```
   ios中多级嵌套flex布局(都是垂直)，可能会导致内层的overflow: auto失效，
即滑动不了
```
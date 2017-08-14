![screen_location](screen_location.jpg)
```
上面的那张图很好的说明了每个方法获得的坐标值或者距离都是从哪里到哪里的。说明一下，图中有三个黑色的框框，最外层的是手机屏幕，

中间层的是ViewGroup，最内层的是ViewGroup中放置的view。

     其实上图中标注的方法可以分为两类，一类是View提供的方法，一类是MotionEvent提供的方法。分别说明如下：

View提供的获取的坐标以及距离的方法：

getTop()           获取到的是view自身的顶边到其父布局顶边的距离

getLeft()           获取到的是view自身的左边到其父布局左边的距离

getRight()        获取到的是view自身的右边到其父布局左边的距离

getBottom()     获取到的是view自身底边到其父布局顶边的距离

 

 

MotionEvent提供的方法：

getX()       获取点击事件距离控件左边的距离，即视图坐标

getY()       获取点击事件距离控件顶边的距离，即视图坐标

getRawX()  获取到的是点击事件距离整个屏幕左边的距离，即绝对坐标

getRawY()  获取到的是点击事件距离整个屏幕顶边的距离，即绝对坐标
```

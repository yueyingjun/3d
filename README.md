# 3d转换#
## 3d转换属性##
1. transfrom
2. transform-origin
3. perspective
4. perspective-origin
5. transform-style
6. backface-visibility

----------------------


# 极坐标和直角坐标系转换公式#
## 极坐标转直角坐标##
<pre>θ 代表天顶角 theta</pre>
<pre>φ 代表方位角  phi</pre>
<code>var x=radius*Math.sin(θ)*Math.cos(φ);
       var z=radius*Math.sin(θ)*Math.sin(φ);
       var y=radius*Math.cos(θ); 
</code>
## 直角坐标转极坐标
<code>
    var r=Math.sqrt(x²+y²+z²);
    var θ=Math.atan(√x²+y²/z)
    var φ=Math.atan(y/x)
</code>
-----------

# 向量的概念
1. 向量是有大小有方向的量
2. 向量的模,指的是向量的大小
<pre>
  模=√x²+y²+z²
</pre> 
3. 单位向量指的是模等于1的向量
<pre>
   x=x轴向量/模
   y=y轴向量/模
   z=z轴向量/模
</pre>

4. css3 rotate3d(x,y,z,角度)
   * x,y,z分别指的是 各个轴的单位向量
   * 角度指的是旋转的角度
5. 角度和弧度的转换公式
   
   <code>角度=弧度*180/PI
   弧度=角度*PI/180
    </code>
-----------

# javascript 三角函数

1. sin\cos\tan\
2. asin\acos\atan\atan2
3. 只接收弧度作为参数
4. Math.atan2(y,x) 用于精确计算各象限的角度
------
 
# transition
1. 在css3 之前 ,浏览器里面所有的动画都是即时完成的
   节省资源
   <pre>
   animate({属性:最终值},5000,ease,function(){})
   </pre>
2. 在css3多个一个变换的选择,默认还是即时完成,添加过渡特性(transition) 
3. 如果想让一个元素的应用过渡特性,
   * 要给改元素 添加 transition 属性
   * 给transition 至少添加两个属性  <code>transition-property  transition-duration</code>
   * 还有一个属性指定动画的方式  <code>transition-timing-function</code>  linear  ease ease-in ease-out ease-in-out  cubic-bezier
   * 还有一个属性指定过渡等待的时间  <code>transition-delay</code>
   * 通过 webkitTransitionEnd 事件 监听过渡完成的状态

 
 
    
    
  

  
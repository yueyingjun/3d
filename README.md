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
  

  
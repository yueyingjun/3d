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
  
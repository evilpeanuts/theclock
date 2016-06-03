## 形状

>矩形

*ctx.fillRect(x y width height)      填充矩形 
*ctx.strokeRect(x y width heigh)     框线矩形 

>圆

* ctx.arc(x,y,r,0,(Math.PI/180)*180);          圆
要有 beginPath();closePath*();

>线

* ctx.benginPath()                      开始一个路径;
* ctx.moveTo(x,y);                      移动画笔到某点 跳过上次路径
* ctx.lineTo(x,y);                      让路径中'拥有'(并不会直接绘制)一条到某点的线
* ctx.rect(x,y,width,height);            让路径中'拥有'(并不会直接绘制)一个矩形
* ctx.fill();                            填充当前路径
* ctx.stroke();                          描边当前路径
* ctx.closePath();                       结束一个路径


<!-- 从画布中清除矩形区域 
 画布的特点，回执上的元素无法更改-->

* ctx.clearRect();

<!-- 清理画布的两种方式 -->
* ctx.clearRect();
* xxx.width=xxx.height=500;

* ctx.quadraticCurveTo(cp1x,cp1y,x,y)     二次贝塞尔x,y为结束点，cp1x,cp1y为控制点。
* ctx.bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)  绘制三次贝塞尔曲线 x,y为结束点，cp1x,cp1y为控制点一，cp2x,cp2y为控制点二。


##　位移（挪动画布）
只保存画布(包含)'状态' 不保存任何图形

* ctx.save();
* ctx.restore();

* ctx.translate(x,y);
* ctx.rotate((Math.PI/180)*30);
* scale();

## 样式

* ctx.fillStyle='rgba(0,0,0,0.8)';
* ctx.strokeStyle="#1b288";

<!-- 阴影 -->
* ctx.shadowOffsetX
* ctx.shadowOffsetY
* ctx.shadowBlur

<!-- 线性渐变 -->
*   var lingrad = ctx.createLinearGradient(0,0,0,150);
*   lingrad.addColorStop(0, '#00ABEB');
*   lingrad.addColorStop(0.5, '#fff');
*   ctx.fillRect(10,10,130,130);
<!-- 径向渐变 -->
*   var RG=ctx.createRadialGradient(x1,x2,r,y1,y2,r);


* ctx.lineWidth
* ctx.lineJoin="inherit"
* ctx.;ineCap="round";
* ctx.setLineDash([10,3]);
* ctx.lineDashOffset=;

* ctx.shadowOffsetX = 2;
* ctx.shadowOffsetY = 2;
* ctx.shadowBlur = 2;
* ctx.shadowColor = "rgba(0, 0, 0, 0.5)";

* ctx.font="48 san_serif";
* crx.textAlign="right";

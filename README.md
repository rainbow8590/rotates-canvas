# rotates-canvas
### 使用canvas做的面向对象的多圆旋转
```
这个特效是使用canvas,用面向对象的方式做的，实现的效果是：
1.创建的圆可以围绕设置的中心点旋转；
2.可以设置每次旋转的的角度；
3.鼠标经过canvas画布停止旋转，离开画布开始旋转
```
### 使用方式
```
封装的代码在html里面，使用的时候可以摘出来，放在单独的js文件中；

创建圆：
var ball = new Ball({
		x: canvas.width/2,
		y: canvas.height/2,
		r: 26,
		lineWidth : 12,
		arcfillColor: 'rgba(150,10,100,.8)',
		strokeColor: 'rgba(0,0,0,.05)',
		textfillColor: '#fff',
		font:'12px aria',
		text:'HTML5',
		isDash: false,
		angle: 0,
		cR: 120,
		addDeg: 0.005
	})
  
  
  参数设置：
  {
    x:              中心点X坐标
    y:              中心点Y坐标
    r:              圆的半径
    lineWidth:      描边的粗细
    arcfillColor:   圆的填充颜色
    strokeColor：   圆的描边颜色
    textfillColor： 文本的颜色
    font：          文本字号字体
    text：          文本内容
    isDash：        描边的类型(虚线)
    angle：         圆创建时的角度
    cR：            圆旋转轨迹的半径
    addDeg：        每次旋转增加的度数
  }
  
```

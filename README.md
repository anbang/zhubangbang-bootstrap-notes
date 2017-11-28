# zhubangbang-bootstrap-notes

bootstrap的基础环境

	<!DOCTYPE html>
	<html lang="zhu-hans">
	<head>
	    <meta charset="UTF-8">
	    <meta name="viewport" content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
	    <meta http-equiv="X-UA-Compatible" content="IE=edag">
	    <link rel="stylesheet" href="lib/bootstrap-3.3.7-dist/css/bootstrap.min.css">
	    <link rel="stylesheet" href="css/public.css">
	    <title>Title</title>
	</head>
	<body>
	<script src="lib/jquery/jquery-1.11.2.min.js"></script>
	<script src="lib/bootstrap-3.3.7-dist/js/bootstrap.min.js"></script>
	</body>
	</html>


BootSrap网格的尺寸,每种网格四种

- col-xs-*  小于768
- col-sm-*	大于768
- col-md-*	中等>992
- col-lg-*	大的>1200

如下中，col-sm-8 中sm可以改为xs、md、lg这样可以改变为缩小到多少px时变为2栏显示

	<div class="container">
	    <div class="row">
	        <div class="col-sm-8">
	            <h1 class="page-header">主体</h1>
	            <p>文字文字文字文字文字文字文字文字文字文字文字文字文字文字</p>
	        </div>
	        <div class="col-sm-4">
	            <h1 class="page-header">主体</h1>
	            <p>文字文字文字文字文字文字文字文字文字文字文字文字文字文字</p>
	        </div>
	    </div>
	</div>



##### API

- 清除浮动
	- clearfix
- 偏移  
	- col-md-offset-4
- 特定尺寸显示隐藏
	- hidden-md		显示
	- visible-xs	隐藏

### 属性

- data-toggle="modal" 			//触发类型 modal | collapse
- data-target="#login-modal" 	//触发的面板区域
- data-dismiss="modal"			//解除的类型，与data-toggle对应
- data-backdrop="false"			//模态框是否有背景

### 其它

- tabindex	//按tab键的显示顺序
- fade		//渐进

##### 导航条相关的

- navbar					//导航条基础类目
	- navbar-header				//顶部区域
		- navbar-brand			//LOGO区域
		- navbar-toggle			//切换的触点
	- navbar-collapse
		- navbar-nav				//导航条的菜单
		- navbar-left				//左对齐
			- navbar-link
			- navbar-text
			- navbar-btn
			- navbar-form
		- navbar-right			//右对齐
- navbar-default			//默认配色
- navbar-inverse			//反转配色
- navbar-fixed-top			//菜单固定在底部
- navbar-fixed-bottom		//菜单固定在底部
- navbar-static-top			//去除navbar的顶部和左右边框


### 模态框
- modal			//基础包裹层类目
	- modal-dialog	//次级包裹
		- modal-content
			- modal-header
			- modal-body
			- modal-footer
	- modal-lg		//控制dialog的宽度-宽
	- modal-sm		//宽度-窄
- data-backdrop="false" //modal同级，可以让模态框没有背景

> 触点区域的（data-toggle="modal"所在的DOM），href="login-form.html"，这样设置，弹窗的modal-content内容会被href所指文件中的文件替换；或者在model统计，加上 data-remote="login-form.html" 也可以达到同样的效果；

** 其它 **
- modal-open
- modal-scrollbar-measure
- modal-title
- glyphicon-modal-window
- modal-backdrop //窗口背景，和modal同级


## 旋转木马 && 幻灯片

- carousel		//最外层基础类
	- carousel-inner		//面板包裹  
		- item
		- active
	- data-ride="carousel" 	//放在carousel-inner同级，
	- carousel-indicators 
	- carousel-control 
	- carousel-caption



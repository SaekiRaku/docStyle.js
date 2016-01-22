# docStyle.js

这是一个JS的外联样式表操作库，可以动态增删、修改CSS3的keyframes的值（您可以打开开发者工具或者查看源码，文档内没有引用任何CSS文件，并且页面元素不含有任何内联样式）。基于MIT协议开源。


This is a JavaScript library for the document style sheets operation, especially for the CSS3 keyframes, you can add, remove and change it dynamic(MT:You can open the developer tools or view the source, without reference to any CSS file in the document, and the page element does not contain any inline styles.). Present by Thomas, released under the MIT license.(I'm not good at English, sorry about the mistake in these sentence.)


> I'm not very good at English, I'd appreciate if somebody can help me translate this document into English or other language,or you can just point out the mistake,thanks so much.


## Get Start / 开始使用

引用js文件，创建一个DIV元素并写一些文字

    <div id="duang">Lorem ipsum dolor sit amet.</div>

然后写JS脚本

    docStyle.addStyle("#duang");
    //添加一个CSS选择器为#duang的外联样式
	docStyle.setStyle("#title","fontSize","32px");
	//设置外联样式的值

Duang，您可以看到div内的文字字号变成了32px，并且不是通过内联样式添加的。
但是，实际上这个类库的主要意义在于操作CSS3的keyframes动画，您可以查看example.html查看docStyle是如何动态修改keyframes的属性的。

## Other API / 其他接口
	hasSelector(selector)
	//选择器是否存在

    setStyle(selector,style,value)
    //修改外联样式
    
	getStyle(selector,style)
	//获取外联样式值
	
	hasStyle(selector,style)
	//指定样式是否存在
	
	setKeyFrames(name,percent,style,value)
	//设置keyframes动画样式
	
	getKeyFrames(name,percent,style)
	//获取keyframes动画样式值
	
	hasKeyFrames(name)
	//指定keyframes动画是否存在
	
	addStyle(selector)
	//添加外联样式
	
	removeStyle(selector)
	//删除外联样式
	
	addKeyFrames(name)
	//添加keyframes动画
	
	removeKeyFrames(name)
	//删除keyframes动画
	
	useKeyFrames(id, className, keyFramesName, time, other)
	//应用keyframes动画
	
	cancelKeyFrames(id, className)
	//取消keyframes动画

## Update Logs / 更新日志
> I think these logs are not very important, so I'm not planing to translate it into other languages.

2016 / 01 / 22
* 添加应用keyFrames动画的函数
* 添加判断选择器，外联样式，keyFrames动画是否存在的函数
* 修正浏览器兼容问题

始于 2016 / 01 / 15

## MIT License / MIT协议

enjoy it, thanks.
感谢您的使用。
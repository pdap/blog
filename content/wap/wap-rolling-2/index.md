#  触摸视差滚动touchSwipe

- pubdate: 2016-2-2 15:01
- tags: wap, javascript

wap-rolliing-2 触摸touchSwipe 系jquery插件，

----------------

## 参考资料

 - [github源码](https://github.com/mattbryson/TouchSwipe-Jquery-Plugin)
 - [官网](http://labs.rampinteractive.co.uk/touchSwipe/demos/index.html)

## 相关js
````html

<script type="text/javascript" src="./js/jquery-1.11.1.min.js"></script>
<script type="text/javascript" src="./js/jquery.touchSwipe.min.js"></script>

````

## Demo

- [示范](./demo.html)


## 结构

`从不同方向触摸灰色区域`

````html
<style type="text/css">
 #test{width: auto;height: auto;background-color: gray;display: block;min-height: 200px;}
</style>

<div id="test">触摸灰色区域</div> 

````

## 基础用法
 
````javascript

$(function() {
  $("#test").swipe( {
    //Generic swipe handler for all directions
    swipe:function(event, direction, distance, duration, fingerCount, fingerData) {
      console.log(event, direction, distance, duration, fingerCount, fingerData);
      $(this).html("你摸了我！！ <br> " + '方向:'+direction+'<br>距离:'+
      distance+'<br>持续时间s:'+duration+'<br>手指总数:'+fingerCount+
      '<br>各个手指的触摸对象:'+JSON.stringify(fingerData));  
    }
  });

  //Set some options later
  $("#test").swipe( {fingers:2} );
});

````
## 方法
-  swipe() 构造函数


## 事件 (TODO:文档翻译成中文)[英文说明](http://labs.rampinteractive.co.uk/touchSwipe/docs/symbols/%24.fn.swipe.html#events)

 - swipe
 - swipeDown
 - .......

----------------
# 文档化介绍

- pubdate: 2016-1-22 12:01
- tags: nico, javascript

简介

----------------

## 声明引用

````html
<script src="http://libs.baidu.com/jquery/1.9.1/jquery.min.js"></script>

````
## 声明结构

````html
<div id='content' >
 测试div 
</div>
````
## 示范js

````javascript
function pcwapcss(pc,wap){
  if (Object.prototype.toString.call(pc) !== '[object Array]'||Object.prototype.toString.call(wap)!== '[object Array]') {
    return false;
  }
     var url = [];
  if (/Android|webOS|iPhone|iPod|BlackBerry|opera mini|opera mobile/i.test(navigator.userAgent)) {
    url = wap;
  } else {
    url = pc;
  }
  for (var i = 0; i < url.length; i++) {
      var link= document.createElement("link");
      link.rel='stylesheet';
      link.type='text/css';
      link.href=url[i];
      document.getElementsByTagName('head')[0].appendChild(link);

  }
}
  // 样式切换
 pcwapcss(['css/pc.css'],['css/wap.css']);

````
## 方法 
### `pcwapcss`
  
  * pcwapcss(`array1`,`array2`) 切换pc wap样式

----------------
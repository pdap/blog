# wap-slider轮播图

- pubdate: 2016-2-2 12:01
- tags: wap, javascript

wapSlider轮播图介绍

----------------

## 引用

````html
<script type="text/javascript" src="http://n2.static.pg0.cn/www/common/base/js/jquery-1.9.1.min.js"></script>
<script src="./js/web_slider.js"></script>
````

## 结构

````html
<style>
        html{color:#333;background:#fff;-webkit-text-size-adjust:none;-ms-text-size-adjust:none;}
        body{font:14px/1 "微软雅黑",arial,helvetica,sans-serif;height:100%; color: #333;background-color: #fff;}
        *{margin:0;padding:0;-webkit-tap-highlight-color: rgba(0,0,0,0);-webkit-user-select: none;text-decoration: none;}
        img{border:0}
        a{text-decoration:none; color: #333;}
        a:link,a:visited,a:hover,a:active{ color: #333; text-decoration: none;}
        i{font-style:normal;font-weight:normal}
        ul{list-style:none}
        :focus{outline:0}
        input[type='search'],button{border:0;-webkit-appearance:none;background-color:transparent;-webkit-border-radius:0;-moz-border-radius:0;border-radius:0; -webkit-user-select: text;}
        ::-webkit-search-decoration,::-webkit-search-cancel-button,::-webkit-search-results-button,::-webkit-search-results-decoration{display:none}
        :-moz-placeholder,::-webkit-input-placeholder{color:#9a9696}
        .wap-slider{ position:relative; width:100%;background:#fff;margin:0; padding:0; padding-bottom:56%; overflow: hidden;}
        .wap-slider .slider{overflow: hidden;visibility: hidden;position:absolute; height: 100%; width:100%;}
        .wap-slider .slider-wrap{overflow:hidden;position:relative; height: 100%;}
        .wap-slider .slider-wrap > div {float: left;width: 100%;position:relative; height: 100%;}
        .slider-wrap img { display: block; width:100%;height: 100%; position: absolute; top: 0; left: 0;}
        .slider-wrap span{ display: block; width: 77.8%; position: absolute; bottom: 0; left:0; height: 25px; line-height: 25px; color: #fff; overflow: hidden;text-overflow: ellipsis;white-space: nowrap; padding-left:2.2%; padding-right: 20%; font-size: 12px; background-color: rgba(0,0,0,.5);}
        .slider-ico{ position:absolute; bottom:9px; right:0; padding-right:8px; margin:0; text-align:right;}
        .slider-ico li{width:6px;height:6px;margin:0 2px;display:inline-block;-webkit-border-radius:3px;border-radius:3px;background-color:#AFAFAF; float: left; margin-top: 10px;}
        .slider-ico li.cur{background-color:#e30228;}
    </style>
<div class="wap-slider" id="wapSlider">
        <div class="slider" id="slider">
            <div class="slider-wrap">
                <div>
                    <a href="javascript:;">
                        <img src="./image/wap/slider_temp1.jpg"/>
                        <span>1《万物生长》范冰冰韩庚生猛“吃你”</span>
                    </a>
                </div>
                <div>
                    <a href="javascript:;">
                        <img src="./image/wap/slider_temp2.jpg"/>
                        <span>2绿箭侠</span>
                    </a>
                </div>
                <div>
                    <a href="javascript:;">
                        <img src="./image/wap/slider_temp1.jpg"/>
                        <span>3《万物生长》范冰冰韩庚生猛“吃你”</span>
                    </a>
                </div>
                <div>
                    <a href="javascript:;">
                        <img src="./image/wap/slider_temp2.jpg"/>
                        <span>4绿箭侠绿箭侠绿箭侠</span>
                    </a>
                </div>
            </div>
        </div>
        <ul class="slider-ico" id="slider-ico">
            <li class="cur"></li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>

````

# js

````javascript

if(document.getElementById('slider-ico')){
            var bullets = document.getElementById('slider-ico').getElementsByTagName('li');
            var banner = Swipe(document.getElementById('slider'), {
                auto: 6000,
                continuous: true,
                disableScroll:false,
                startSlide: 0,
                callback: function(pos) {
                    if(document.getElementById('slider-ico').getElementsByTagName('li').length == 2){
                        pos = pos%2;
                    }
                    var i = bullets.length;
                    while (i--) {
                        bullets[i].className = ' ';
                    }
                    bullets[pos].className = 'cur';
               }
           })
        }

````

----------------
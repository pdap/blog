# 滑动视差滚动zepto

- pubdate: 2016-2-2 13:01
- tags: wap, javascript

wap-rolliing-1 滑动视差滚动 系zepto插件
 

----------------

## touch.js部分说明
 
````html

<script src="./js/zepto.min.js"></script>
<script src="./js/touch.js"></script>
 
        
````

## demo

- [示范](./demo.html)


## 结构

````
<div>
    <div class="page page-1-1 page-current">
        <div class="wrap">
            <img class="img_1 pt-page-moveFromTop page-current" src="./image/cover.png">
            <img class="img_2 pt-page-moveFromLeft page-current" src="./image/wording_cover.png">
            <img class="img_3 pt-page-moveIconUp page-current" src="./image/icon_up.png">
        </div>
    </div>
    <div class="page page-2-1 hide">
        <div class="wrap">
            <img class="img_1 pt-page-moveFromBottom" src="./image/wording.png">
            <img class="img_2 pt-page-moveCircle" src="./image/circle.png">
            <img class="img_3 pt-page-moveFromLeft" src="./image/people.png">
            <img class="img_4 pt-page-scaleUp" src="./image/dot1.png">
            <img class="img_5 pt-page-scaleUp" src="./image/check_develop.png">
            <img class="img_6 pt-page-moveIconUp" src="./image/icon_up.png">
            <img class="img_7 pt-page-scaleUp" src="./image/floating_develop.png">
        </div>
    </div>
    <div class="page page-2-2 hide">
        <div class="wrap">
            <img class="img_1 pt-page-flipInLeft hide" src="./image/introduction.png">
            <img class="img_2 pt-page-flipInLeft hide" src="./image/btn_develop.png">
            <img class="img_3 pt-page-flipInLeft hide" src="./image/dot2.png">
            <img class="img_6 pt-page-moveIconUp hide" src="./image/icon_up.png">
        </div>
    </div>
    <div class="page page-2-3 hide">
        <div class="wrap">
            <img class="img_1 pt-page-flipInLeft hide" src="./image/introduction.png">
            <img class="img_2 pt-page-flipInLeft hide" src="./image/btn_develop.png">
            <img class="img_3 pt-page-flipInLeft hide" src="./image/dot2.png">
            <img class="img_6 pt-page-moveIconUp hide" src="./image/icon_up.png">
        </div>
    </div>
    <div class="page page-3-1 hide">
        <div class="wrap">
            <img class="img_1 hide pt-page-moveFromBottom" src="./image/wording_design.png">
            <img class="img_2 hide pt-page-moveCircle" src="./image/circle-design.png">
            <img class="img_3 pt-page-moveFromBottom hide" src="./image/people_design.png">
            <img class="img_4 hide pt-page-scaleUp" src="./image/dot1.png">
            <img class="img_5 hide pt-page-scaleUp" src="./image/check_design.png">
            <img class="img_6 hide pt-page-moveIconUp" src="./image/icon_up.png">
            <img class="img_7 hide pt-page-scaleUp" src="./image/floating_design.png">
        </div>
    </div>
    <div class="page page-3-2 hide">
        <div class="wrap">
            <img class="img_1 hide pt-page-flipInLeft" src="./image/introduction_design.png">
            <img class="img_2 hide pt-page-flipInLeft" src="./image/btn_design.png">
            <img class="img_3 hide pt-page-flipInLeft" src="./image/dot2.png">
            <img class="img_6 hide pt-page-moveIconUp" src="./image/icon_up.png">
        </div>
    </div>
    <div class="page page-4-1 hide">
        <div class="wrap">
            <img class="img_1 hide pt-page-moveFromBottom" src="./image/wording_production.png">
            <img class="img_2 hide pt-page-moveCircle" src="./image/circle-production.png">
            <img class="img_3 pt-page-moveFromRight" src="./image/people_production.png">
            <img class="img_4 hide pt-page-scaleUp" src="./image/dot1.png">
            <img class="img_5 hide pt-page-scaleUp" src="./image/check_production.png">
            <img class="img_6 hide pt-page-moveIconUp" src="./image/icon_up.png">
            <img class="img_7 hide pt-page-scaleUp" src="./image/floating_production.png">
            <img class="img_8 hide pt-page-scaleUp" src="./image/pic_shadow_production.png">
        </div>
    </div>
    <div class="page page-4-2 hide">
        <div class="wrap">
            <img class="img_1 hide pt-page-flipInLeft" src="./image/introduction_production.png">
            <img class="img_2 hide pt-page-flipInLeft" src="./image/btn_production.png">
            <img class="img_3 hide pt-page-flipInLeft" src="./image/dot2.png">
            <img class="img_6 hide pt-page-moveIconUp" src="./image/icon_up.png">
        </div>
    </div>
    <div class="page page-5-1 hide">
        <div class="wrap">
            <img class="img_1 hide pt-page-rotateCubeBottomIn" src="./image/pic_back.png">
            <img class="img_2 hide pt-page-rotateCubeTopIn" src="./image/btn_join.png">
        </div>
    </div>
</div>   

````

 

 

----------------
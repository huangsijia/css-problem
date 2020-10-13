##  移动端适配
    1、flexible:
    <script src="http://g.tbcdn.cn/mtb/lib-flexible/0.3.4/??flexible_css.js,flexible.js"></script>
    <style>
    html,body{font-size:12px;}
    [data-dpr="2"] html,body{font-size:24px;}
    [data-dpr="2"] html,body{font-size:36px;}
    </style>


## ￥
      &yen;

## 初始化清空
      /** 清除内外边距 **/
      body, h1, h2, h3, h4, h5, h6, hr, p,
      blockquote, /* structural elements 结构元素 */
      dl, dt, dd, ul, ol, li, /* list elements 列表元素 */
      pre, /* text formatting elements 文本格式元素 */
      form, fieldset, legend, button, input, textarea, /* form elements 表单元素 */
      th, td, /* table elements 表格元素 */
      img/* img elements 图片元素 */{
        border:medium none;
        margin: 0;
        padding: 0;
      }
      /** 设置默认字体 **/
      body,button, input, select, textarea {
        font: 12px/1.5 '宋体',tahoma, Srial, helvetica, sans-serif;
      }
      h1, h2, h3, h4, h5, h6 { font-size: 100%; }
      em{font-style:normal;}
      /** 重置列表元素 **/
      ul, ol { list-style: none; }
      /** 重置超链接元素 **/
      a { text-decoration: none; color:#333;}
      a:hover { text-decoration: underline; color:#F40; }
      /** 重置图片元素 **/
      img{ border:0px;}
      /** 重置表格元素 **/
      table { border-collapse: collapse; border-spacing: 0; }
      /** 清除内外边距 **/
## 悬浮 left不要设置
    .bot {
    width: 100%;
    max-width: 750px;
    height: 5rem;
    position: fixed;
    bottom: 0;
    background: rgba(0,0,0,.7);
    z-index: 99;
     }
     
## 渐变遮挡
    .list .w92:before{content:'';width:100%;height:20px;display:block;background-image:linear-gradient(rgba(16,102,201,1) 60%,rgba(16,102,201,0) 100%);background-image:-webkit-linear-gradient(rgba(16,102,201,1) 60%,rgba(16,102,201,0) 100%);position:relative;z-index:5}
    .list .w92:after{content:'';width:100%;height:20px; display:block;background-image:linear-gradient(rgba(16,102,201,0) 0,rgba(16,102,201,1) 50%); background-image:-webkit-linear-gradient(rgba(16,102,201,0) 0,rgba(16,102,201,1) 50%);position:absolute;bottom:0;z-index:5}
    background-image: linear-gradient(to bottom, $red, $gradientRed);
    background-image: -webkit-gradient(linear, 50% 0%, 50% 100%, from($red), to($gradientRed));
    
## 转盘排版
    .turn .dish ul{width:100%;height:90%;position:absolute;top:5.2%;left:0;}
    .turn .dish ul li{position:absolute;left:33%;top:0;width:34%;height:50%;text-align:center;transform-origin:center bottom;-webkit-transform-origin:center bottom;}    
    .turn .dish ul li:nth-child(1){transform:rotate(22.5deg);-webkit-transform:rotate(22.5deg);}
    .turn .dish ul li:nth-child(2){transform:rotate(68deg);-webkit-transform:rotate(68deg);}
    .turn .dish ul li:nth-child(3){transform:rotate(113deg);-webkit-transform:rotate(113deg);}
    .turn .dish ul li:nth-child(4){transform:rotate(158deg);-webkit-transform:rotate(158deg);}
    .turn .dish ul li:nth-child(5){transform:rotate(202deg);-webkit-transform:rotate(202deg);}
    .turn .dish ul li:nth-child(6){transform:rotate(247deg);-webkit-transform:rotate(247deg);}
    .turn .dish ul li:nth-child(7){transform:rotate(292deg);-webkit-transform:rotate(292deg);}
    .turn .dish ul li:nth-child(8){transform:rotate(337deg);-webkit-transform:rotate(337deg);}
    
## a标签点击阴影
      a{-webkit-tap-highlight-color:rgba(0,0,0,0);-webkit-touch-callout:none;}
## 阴影
box-shadow:0 0 15px 0 rgba(0, 0, 0, 0.2), 0 25px 30px -20px rgba(57, 114, 0, 0.6)
      
## 去除手机号
      <meta content="telephone=no" name="format-detection">
      
## chrome跨域
      --disable-web-security
       --args --disable-web-security --user-data-dir
## 居中
      transform:translate(-50%,-50%);
## 渐变
      border-width:1px;border-style:solid;border-image:linear-gradient(#99c0f1, #5377d7) 30 30;
      background-image:linear-gradient(to right,red,blue)
## meta
      <meta content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no" name="viewport"><!-- H5页面窗口自动调整到设备宽度，并禁止用户缩放页面-->
      <meta content="yes" name="apple-mobile-web-app-capable"><!-- 当网站添加到主屏幕快速启动方式，可隐藏地址栏，仅针对ios的safari-->
      <meta content="black" name="apple-mobile-web-app-status-bar-style"><!-- 将网站添加到主屏幕快速启动方式，仅针对ios的safari顶端状态条的样式-->
      <meta content="telephone=no" name="format-detection"><!-- 忽略将页面中的数字识别为电话号码-->
      <meta content="email=no" name="format-detection"><!-- 忽略Android平台中对邮箱地址的识别-->
      
## meta
      apple-mobile-web-app-capable删除默认的苹果工具栏和菜单栏。
      apple-mobile-web-app-status-bar-style作用是控制状态栏显示样式
      
## css计算大小
      $uiWidth:375px;
      @function pxToRem($px){
        @return 10 * $px/$uiWidth/2 * 1px;
      }
      @mixin screen($res-min, $res-max) {
        @media screen and (min-width: $res-min+px) and (max-width: $res-max+px) {
          .recharge {
            .page-part {
              margin-top: pxToRem(20px) * ($res-min/10);
                        }
                    }
        }
        @include screen(320,568);
        
## css加
      span{width:5rem;height:5rem;border:.4rem solid #bcb9b9;border-radius:50%;-webkit-border-radius:50%;display:block;position:absolute;left:50%;top: 50%;margin-left:-2.5rem;margin-top:-2.5rem;}
      span:before{content:'';width:.6rem;height:2rem;border-radius:1rem;-webkit-border-radius:1rem;background:#bcb9b9;display:block;position:absolute;top:50%;left:50%;z-index:0;margin-top:-1rem;margin-left:-.3rem;}
      span:after{content:'';width:2rem;height:.6rem;border-radius:1rem;-webkit-border-radius:1rem;background:#bcb9b9;display:block;position:absolute;top:50%;left:50%;z-index:1;margin-top:-.3rem;margin-left:-1rem;}
      
## input的number可以输入e
      type="number" onkeypress="return (/[\d]/.test(String.fromCharCode(event.keyCode)))"
 
## 透明
      transparent
## 点点点
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
    display: inline-block;
    
## 灰色 
    opacity: .4;
    filter: alpha(opacity=40);
    filter: url(data:image/svg+xml;utf8,#grayscale);
    -webkit-filter: grayscale(100%);
    filter: grayscale(100%);
    filter: gray;
    filter: progid:DXImageTransform.Microsoft.BasicImage(grayscale=1);
## hover 彩色
    opacity: 1;
    filter: alpha(opacity=0);
    -webkit-filter: grayscale(0);
    filter: grayscale(0);
    filter: gray(0);
    filter: progid:DXImageTransform.Microsoft.BasicImage(grayscale=0);
    filter: progid:DXImageTransform.Microsoft.gradient(startColorstr=#E5ffffff,endColorstr=#E5ffffff)

## inpout记住密码
      autocomplete="new-password"
## 居中
    -webkit-transform: translate(0,-50%);
    transform: translate(0,-50%);

## 对号
      <div class="check"></div>
      .check{
      background: #e53344;
      display: inline-block;
      width: 10px;
      height: 2px;
      margin: 2.4rem 1.2rem 0 0;
      bline-height: 0;
      font-size: 0;
      vertical-align: middle;
      -webkit-transform: rotate(45deg);
      }
      .check:after{
          content: '/';
          display: block;
          width: 20px;
          height: 2px;
          background: #e53344;
          -webkit-transform: rotate(-90deg) translateY(-50%) translateX(50%);
      }
## input解决浏览器会自动填充密码的问题
      autocomplete="new-password"
      
## 微信二维码生成
      open.weixin.qq.com/qr/code/?username=微信号
## 强制跳转
      <meta http-equiv="Refresh" content="0; url=http://bxjr.com/topic/security/" />
##  table自定义border
      border-collapse: collapse;
## border image
    border: 10px solid transparent;
    border-image: url(../images/border-img.png) 10 10 round;
    -webkit-border-image: url(../images/border-img.png) 10 10 round;
    border-bottom: 0;
    border-bottom-image: 0;
    -webkit-border-bottom-image: 0;

## 翻转和平滑
/*.product-con:hover .title-tag{-webkit-animation:flip 1s 1;animation:flip 1s 1;}*/
/*@keyframes flip{from{transform:rotateX(0deg); -ms-transform:rotateX(0deg); -moz-transform:rotateX(0deg); -webkit-transform:rotateX(0deg); -o-transform:rotateX(0deg);} to{transform:rotateX(360deg); -ms-transform:rotateX(360deg); -moz-transform:rotateX(360deg); -webkit-transform:rotateX(360deg); -o-transform:rotateX(360deg);}}*/
.product-con .title-tag{position: relative;}
.product-con .title-tag:after{content:"";position: absolute; top: 0; left: -25px; width: 30px; height: 22px; -webkit-transform: skew(-25deg); -moz-transform: skew(-25deg); -o-transform: skew(-25deg); -ms-transform: skew(-25deg);background-image: -webkit-linear-gradient(0deg, rgba(255, 255, 255, 0.5), rgba(255, 255, 255, 0.5), rgba(255, 255, 255, 0));}
.product-con:hover .title-tag:after{left:84px; -webkit-transition: 2s; -moz-transition: 2s; -ms-transition: 2s; -o-transition: 2s; transition: 2s;}


## iPhoneX适配
            第一步：设置网页在可视窗口的布局方式
            ios11新增 viweport-fit 属性，使得页面内容完全覆盖整个窗口：

            <meta name="viewport" content="width=device-width, viewport-fit=cover">
            第二步：页面主体内容限定在安全区域内
            env() 和 constant()ios11新增特性

            ● safe-area-inset-left：安全区域距离左边边界距离
            ● safe-area-inset-right：安全区域距离右边边界距离
            ● safe-area-inset-top：安全区域距离顶部边界距离
            ● safe-area-inset-bottom：安全区域距离底部边界距离

            这里我们只需要关注 safe-area-inset-bottom 这个变量，因为它对应的就是小黑条的高度（横竖屏时值不一样）。

            body {
                padding-bottom: constant(safe-area-inset-bottom);
                padding-bottom: env(safe-area-inset-bottom);
            }
            第三步：fixed 元素的适配
            ● 类型一：fixed 完全吸底元素（bottom = 0）

            {
                padding-bottom: constant(safe-area-inset-bottom);
                padding-bottom: env(safe-area-inset-bottom);
            }
            ● 类型二：fixed 非完全吸底元素（bottom ≠ 0），比如 “返回顶部”、“侧边广告” 等

            {
                margin-bottom: constant(safe-area-inset-bottom);
                margin-bottom: env(safe-area-inset-bottom);
            }
            第四步：如果我们只希望 iPhoneX 才需要新增适配样式，我们可以配合 @supports 来隔离兼容样式

            @supports (bottom: constant(safe-area-inset-bottom)) or (bottom: env(safe-area-inset-bottom)) {
                div {
                    margin-bottom: constant(safe-area-inset-bottom);
                    margin-bottom: env(safe-area-inset-bottom);
                }
            }
            
## 鼠标定义图片
      a {
        Cursor: url("../images/a1.png") 4 12, auto;
      }

      a:active {
        cursor: url("../images/a2.png") 4 12, auto;
      }
      
## 居中title
      .title{width:70%;height:3rem;line-height: 3rem;margin:4rem auto 1rem;font-size:1.6rem;text-align: center;color:#d89b00;font-size: 30px;}
        .title h3{width:50%;}
        .title i{width:25%;margin-top: 1.4rem;height:1px;background:#e3baa4;position: relative;}
        .title i:before{content:"";width:14px;height:14px;background:#e3baa4;display:block;position:absolute;top:0;}
        .title i.before:before{right:0;transform:rotate(45deg) translate(0,-50%);-webkit-transform:rotate(45deg) translate(0,-50%);}
        .title i.after:before{left:0;transform:rotate(45deg) translate(-50%,0);-webkit-transform:rotate(45deg) translate(-50%,0);}
        
## IE8 transform
      http://www.useragentman.com/IETransformsTranslator/
      
## css animate
      https://daneden.github.io/animate.css/
      
      
## table border
      <table border="1">
      table,table tr th, table tr td { border:1px solid #e3e3e3; }
      table{border-collapse: collapse;}
      
## 右边宽度固定，左边自适应
      第一种
      <style>
      body{
          display: flex;
      }
      .left{
          background-color: rebeccapurple;
          height: 200px;
          flex: 1;
      }
      .right{
          background-color: red;
          height: 200px;
          width: 100px;
      }
      </style>
      <body>
          <div class="left"></div>
          <div class="right"></div>
      </body>
      第二种
      <style>
    div {
        height: 200px;
    }
    .left {
        float: right;
        width: 200px;
        background-color: rebeccapurple;
    }
    .right {
        margin-right: 200px;
        background-color: red;
    }
      </style>
      <body>
          <div class="left"></div>
          <div class="right"></div>
      </body>
## 水平居中
      第一种
      #container{
        position:relative;
    }

    #center{
        width:100px;
        height:100px;
        position:absolute;
        top:50%;
        left:50%;
        transform: translate(-50%,-50%);//或者第二种修改margin一处 margin:-50px 0 0 -50px;
        background: red;
    }
    第三种
        position:absolute;
        margin:auto;
        top:0;
        bottom:0;
        left:0;
        right:0;
    第四种 ie8不支持
    display:flex;
    justify-content:center;
    align-items: center;
    
## box-shadow圆形
      box-shadow: 0 30px 40px -20px rgba(114,82,0,.2);
      
## img不可点击
      img{
           -webkit-user-select: none;  /* Chrome all / Safari all */
          -moz-user-select: none;     /* Firefox all */
          -ms-user-select: none;      /* IE 10+ */
      }
      
## 自动跳转代码如下：
      <meta http-equiv="Refresh" content="1; url=http://www.baidu.com"/>
      
## IE透明
      filter:progid:DXImageTransform.Microsoft.gradient(startcolorstr=#7F000000,endcolorstr=#7F000000);

## 实现瀑布流布局的函数
        function waterfall() {
            var items = $("div.item"); //获取到所有的类名为item的元素
            var postop = []; //这个数组用来存放item定位的高度
            var itemWidth = items.eq(0).width(); //宽度都是一样的,所以随便获取一个就行
            var spaceWidth = $(".waterfall").width() - itemWidth * 2;

            items.each(function (index, elem) {
                var targetItemTop = $(elem).height(); //遍历所有item并获取高度

                if (index < 2) {
                    //如果是在第一行
                    postop[index] = targetItemTop; //把高度直接加入数组中
                    $(elem).css({
                        "left": itemWidth * index + (index % 2 === 0 ? 0 : spaceWidth), //设置left
                        "top": 0 //和top
                    });
                } else {
                    //其他行
                    var mintop = Math.min.apply(null, postop); //获取数组中最小的一个
                    var minindex = $.inArray(mintop, postop); //获取到数组最小值对应的排序

                    $(elem).css({
                        "top": mintop + 20, //设置top为数组中最小值
                        "left": itemWidth * minindex + (minindex % 2 === 0 ? 0 : spaceWidth) //设置left
                    });
                }
                postop[minindex] += $(elem).height() + 20; //更新数组
            });

            $(".waterfall").css({height: Math.max.apply(null, postop)});
        }

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
      
## 去除手机号
      <meta content="telephone=no" name="format-detection">
      
## chrome跨域
      --disable-web-security
       --args --disable-web-security --user-data-dir
## 居中
      transform:translate(-50%,-50%);
## 渐变
      border-width:1px;border-style:solid;border-image:linear-gradient(#99c0f1, #5377d7) 30 30;
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

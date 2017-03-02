
## 悬浮 left不要设置
    <div class="bot">我浮在最下方</div>
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
    

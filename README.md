
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

    

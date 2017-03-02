# h5界面，最大宽度750px,悬浮在最下方的div不超过750px，left不要设置
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

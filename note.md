            <section class="popular">
                <h2 class="section-title">熱銷商品</h2>
                <div class="arrow-left arrow"><i class="fas fa-arrow-alt-circle-left"></i></div>
                <div class="popularCtn">
                    <div class="popular-slider">
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0021.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0006.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo//image_product/BD0401.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/CA0041.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo//image_product/AH0401.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo//image_product/FA0301.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo//image_product/AI0301.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/AE0081.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0029.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0028.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0022.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                        <div class="item">
                            <div class="top-img">
                                <img src="https://k-photo.smarter.com.tw/Photo/image_product/DIS0022.png" alt="">
                            </div>
                            <div class="text-wrapper">
                                <p class="pop-title">SOS全能修復霜</p>
                                <p class="pop-size">150ml</p>
                                <p class="pop-price">NT$1399</p>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="arrow-right arrow"><i class="fas fa-arrow-alt-circle-right"></i></div>
            </section>

                <script>

        function getStyle(obj,name){
    if(window.getComputedStyle){
        return getComputedStyle(obj,null)[name];
    }else{
        return obj.currentStyle[name];
    }
}

function move(obj,attr,target,speed,callback){
    var current = parseInt(getStyle(obj,attr));
    if(current >target){
        speed = -speed;
    }
    clearInterval(obj.timer);
    obj.timer = setInterval(function(){
        var oldValue = getStyle(obj,attr);
        var currentValue = parseInt(oldValue) + speed;
        if((speed<0&&currentValue<target)||(speed>0&&currentValue>target)){
            currentValue = target;
        }
        obj.style[attr] = currentValue +"px";
        if(currentValue == target){
            clearInterval(obj.timer);
            callback && callback();
        }
    },15)      
}
var sliderCtn = document.querySelector(".popularCtn");
var sliderList = document.querySelector(".popular-slider");
var slides = document.querySelectorAll(".item");
var prev = document.querySelector(".arrow-left");
var next = document.querySelector(".arrow-right");
var index = 0;
        next.onclick = function(){
            index++;
            if(index>1){
                index =0;
                sliderList.style.left = 0+"px";
            }
            move(sliderList,"left",-1372*index,10);
        }
        prev.onclick = function(){
            index--;
            if(index<0){
                index = 1;
                sliderList.style.left = -1372+"px";
            }
            move(sliderList,"left",-1372*index,10);
        }
    </script>

            .popular .item{
            overflow: hidden;
            width:220px;
            height:300px;
            border: 1px solid #000;
            margin:0 5px;
        }
        .popular .item:first-child{
            margin-left: 0;
        }
        .arrow{
            position: absolute;
            font-size: 35px;
            z-index: 9999;
            top:30%;
            transform: translateY(-50%);
            cursor: pointer;
        }
        .arrow-left{
            left: 0;
        }
        .arrow-right{
            right:0;
        }
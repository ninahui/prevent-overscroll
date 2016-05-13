微信浏览器禁止页面下拉查看网址（不影响页面内部scroll）

此类事件是手机touchmove默认事件行为，可以通过js代码隐藏事件：

$(‘body’).on(‘touchmove’, function (event) {event.preventDefault();});
or
document.addEventListener('touchmove', function(e){e.preventDefault()}, false);
但这样往往会把页面原生的scroll效果也一同去掉了，下面的代码可以完美解决这个问题：

文／我是7号_frank（简书作者）
原文链接：http://www.jianshu.com/p/2eddee561971
著作权归作者所有，转载请联系作者获得授权，并标注“简书作者”。

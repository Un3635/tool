1. FastClick用法 https://majing.io/posts/10000007721218
2.  qrcode.min.js 生成二维码 事例
```
(function () {
        var wrap = document.getElementById('qrcode');
        var href = window.location.href.replace('xx.html', 'xxx.html?inviteCode=4CFVBERT');
        var qrcode = new QRCode(document.getElementById("qrcode"), {
          text: href,
          width: wrap.clientWidth,
          height: wrap.clientWidth,
          colorDark : "#000000",
          colorLight : "#ffffff",
          correctLevel : QRCode.CorrectLevel.H
        });
    })();
    
    // https://cdn.bootcss.com/qrcode-generator/1.4.1/qrcode.js 会受url长度的限制
```

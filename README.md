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
3.  moment-with-locales.js 事例
```
        $('<div>').html(moment(data[i].receiveTime).format("YYYY.MM.DD HH:mm"))
```
4. wxcharts 事例
```
 this.chart = new Charts({
      canvasId: 'canvas',
      type: 'line',
      extra: {
        lineStyle: 'curve', //线条的形状（弧形）
        column: {
          width: 10
        }
      },
      title: {
        // name: '70%',
        // color: '#7cb5ec',
        // fontSize: 25
      },
      categories: ['剁椒鱼头', '清蒸鲈鱼', '开胃鱼头', '酸辣土豆丝', '干锅土鸡', '西红柿蛋汤', '口水鸡', '香菇菜心', '酒酿丸子', '椰奶', '剁椒鱼头1', '清蒸鲈鱼2'],
      series: [{
        name: '饿了么',
        data: [40, null, 44, 12, 30, 18, 24, 22, 20, 8],
        format: function (val) {
          return val;
        }
      }, {
        name: '美团',
        fontSize: '30px',
        data: [38, 40, 42, 10, 30, 20, 24, 22, 20, 8],
        format: function (val) {
          return val;
        }
      }],
      yAxis: {
        format: function (val) {
          return val + '元';
        }
        // fontColor: "#8a6e57"
      },
      xAxis: {
        axisTick: { length: 50 }
      },
     
      width: wx.getSystemInfoSync().windowWidth,
      height: wx.getSystemInfoSync().windowHeight/2,
      totalWidth: Number(_.data.dataLength) * (_.data.windowWidth / 5.5) > _.data.windowWidth ? _.data.dataLength * (_.data.windowWidth / 5.5): _.data.windowWidth,
      animation: true,
      enableScroll: true, // 使得categories非响应布局
    });
    借鉴: https://www.cnblogs.com/mmykdbc/p/8927329.html
   
```

<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8" />
    <title></title>
    <style>
        p {
            text-indent: 2em;
        }

        img {
            position: absolute;
            right: 50px;
            top: 150px;
        }
    </style>
    <style>
        a:link {
            text-decoration: none;
            color: blue;
        }
        /*未访问的链接显示为蓝色，text-decoration:none将下划线隐藏*/
        a:visited {
            color: black;
        }
        /*用户已访问过的链接显示黑色*/
        a:hover {
            color: slategray;
        }
        /*鼠标放置在链接上时显示为粉色*/
        a:active {
            color: yellow;
        }
        /* 链接被点击那一刻显示黄色 */
    </style>
    <style>
        .button {
            undefined font: bold 11px Arial;
            text-decoration: none;
            background-color: #bad0f5;
            color: #000000;
            padding: 2px 6px 2px 6px;
            border-top: 3px solid #808080;
            border-right: 3px solid #808080;
            border-bottom: 3px solid #808080;
            border-left: 3px solid #808080;
        }

    </style>
</head>
<body>

    <script type="text/javascript" src="http://webapi.amap.com/maps?v=1.3&key=8847c5413ff11a3f0aab665c326f1600"></script>

    <div id="container" style="width:809px; height:500px"></div>

    <script>

        //对于地图的自定义，属性有很多，只列举三个
        var map = new AMap.Map('container', {
            zoom: 6,//缩放级别
            center: [112.73, 38.42],//地图显示中心点坐标，如果没有center属性，则会定位到你当前所处的位置
            viewMode: '3D'//使用3D视图
        });
        var marker = new AMap.Marker({
            icon: "//a.amap.com/jsapi_demos/static/demo-center/icons/poi-marker-default.png",
            position: [112.73, 38.42],
            offset: new AMap.Pixel(-13, -30)
        });

        // 将创建的点标记添加到已有的地图实例：
        map.add(marker);

    </script>

    <img src="https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fci.xiaohongshu.com%2Ffa4ee42b-f270-989a-6a01-275be10968be%3FimageView2%2F2%2Fw%2F1080%2Fformat%2Fjpg&refer=http%3A%2F%2Fci.xiaohongshu.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1649516599&t=826e9ff5dff3140a181a49e9cdc6cc0b" width="420" height="300" />
    
    
    <a href="https://www.sxxz.gov.cn/zjxz/" style="margin-left:970px;margin-top:500px" class="button">忻州市简介</a>
</body>
</html>

    

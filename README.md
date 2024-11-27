# Auto Set Bilibili Video in HTML
真·仅需一行代码, 快速解析并设置&lt;video>的Bilibili视频链接  
***Created by [CNZW](https://cnzw.us.kg/)***

### 1. 在&lt;head>标签中添加JavaScript文件
```html
<script src="./main.js"></script>
```
或
```html
<script src="https://api.cnzw.us.kg/js/set_bili_video.js"></script>
```
### 2. 在&lt;video>标签中添加指定属性
```html
<video data-bili-id=""></video>
```
其中, data-bili-id是视频的AV或BV号

### 示例代码
```html
<!DOCTYPE html>
<html lang="zh-cn">

<head>
    <script src="https://api.cnzw.us.kg/js/set_bili_video.js"></script>
</head>

<body>
    <video data-bili-id="BV1Ag4y1b7pa"></video>
</body>

</html>
```
### 示例效果
![image](https://github.com/user-attachments/assets/147ab648-0e6a-4d29-82f2-153db4cc9f31)


>[!NOTE]
>此项目所使用的API: https://api.dyqvideo.com/download/url/get  
>经测试, 该API只能解析的视频只有360P的清晰度, 如果你有更好的API接口, 可以自行替换  
>请求方法: **POST**  
>请求参数:
>```json
>"url": "这里替换为视频链接",
>"videoChannel": "BILI_BILI"
>```
>返回参数:
>```json
>{
>    "data": {
>        "downloadUrl": "视频链接",
>        "name": "视频标题"
>    },
>    "code": 0,
>    "msg": null
>}
>```

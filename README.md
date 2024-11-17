# Auto Set Bilibili Video in HTML
仅需一行代码, 快速解析并设置&lt;video>的Bilibili视频链接
### 1. 在&lt;head>标签中添加JavaScript文件
```html
<script src="./main.js"></script>
```
或
```html
<script src="https://api.cnzw.us.kg/js/set_bili_bv_video.js"></script>
```
### 2. 在&lt;video>标签中添加指定属性
```html
<video data-bili-bv="" data-bili-p=""></video>
```
其中, data-bili-bv是视频的BV号(必要), data-bili-p是视频的集数(非必要, 默认为1)

### 示例代码
```html
<!DOCTYPE html>
<html lang="zh-cn">

<head>
    <script src="https://api.cnzw.us.kg/js/set_bili_bv_video.js"></script>
</head>

<body>
    <video data-bili-bv="BV1Ag4y1b7pa" data-bili-p="1"></video>
</body>

</html>
```
### 示例效果
![image](https://github.com/user-attachments/assets/9317b1a8-36ed-407d-8976-ed1322bb69ee)


### 缺点
由于权限问题, 有时可能会出现短暂由403 Forbidden导致的无法播放情况

>[!NOTE]
>此项目所使用的API: [INJAHOW](https://api.injahow.cn/bparse/)

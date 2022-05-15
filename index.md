<html>
<head>
<title>Steak Web</title>
<meta charset="utf-8">
<meta content="width=device-width, initial-scale=1.0, maximum-scale=3.0, user-scalable=1" name="viewport">
<meta name="description" content="Steak Web由牛排吖制作，是一个为上课摸鱼的同志们量身打造的起始页。Steak Web以最简洁的界面容纳了内置导航栏、超链接网站捷径、伪息屏等实用功能，让您的网上冲浪体验更加舒心(bushi)。">
<link rel="shortcut icon" href="pic/icon.png">
<link rel="apple-touch-icon" href="pic/icon.png">
<style>
.btn {border:1pt solid #fff;background:rgba(0,0,0,0.2);border-radius:6px;width:25%;height:45px;font-size:80%;font-weight:light;color:#fff;}
.btn:hover {border:1pt solid #000;background:rgba(0,0,0,0.3);border-radius:6px;width:25%;height:45px;font-size:80%;font-weight:light;color:#000;}
</style>
</head>
<body id="bg" onload="load();">
<div style="width:100%;height:100%;position:fixed;background:rgba(0,0,0,0.3);text-align:center;">

<div style="display:none;width:100%;height:100%;position:fixed;background:rgba(0,0,0,0.3);text-align:center;z-index:100;" id="fs">
<div id="loadb" style="width:11vw;height:11vw;top:35vh;left:45vw;position:relative;background:rgba(0,0,0,0.4);border-radius:6px;overflow:hidden;">
<img style="width:80%;border:0px;transform:rotateX(0deg);transform-origin:50% 50%;" src="pic/load.png" id="icon"></img>
<br>
<span style="color:#efefef;font-size:125%;font-weight:light;">加载中...</span>
</div>
</div>

<div style="position:relative;top:25vh;">
<p align="center">
<span style="color:white;font-size:260%;font-weight:light;">Steak Web</span>
<br>
<span style="color:white;font-size:90%;font-weight:light;"> ——为摸鱼的同志们量身打造</span>
</p>
</div>
<div style="position:relative;top:30vh;">
<input type="button" class="btn" value="开始摸鱼awa" onclick="SFish();">
<p>
<input type="button"  class="btn" value="算了认真学习" onclick="window.close();">
</div>
</div>

</body>
<script>
function load(){
var bg = document.getElementById("bg");
var x = Math.floor(Math.random()*4);
if(x==0){
bg.style = "margin:0px;padding:0px;width:100%;background:url(pic/0.png);background-position:bottom;background-size:contain";
}
if(x==1){
bg.style = "margin:0px;padding:0px;width:100%;background:url(pic/1.png);background-position:bottom;background-size:contain";
}
if(x==2){
bg.style = "margin:0px;padding:0px;width:100%;background:url(pic/2.png);background-position:bottom;background-size:contain";
}
if(x==3){
bg.style = "margin:0px;padding:0px;width:100%;background:url(pic/3.png);background-position:bottom;background-size:contain";
}
}

function SFish(){
var div = document.getElementById("fs");
div.style.display = "block";
setTimeout("rotated();",0);
setTimeout("toUrl();",500);
}
var c=0;
function rotated(){
var x = document.getElementById("icon");
c+=3;
x.style.transform="rotateY(" + c + "deg)";
setTimeout("rotated();",10);
}
function toUrl(){
window.open("main.html");
}
</script>
</html>












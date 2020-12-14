## JQuery
1. JQuery是一个JavaScript的轻量级的函数库，简化js编程。
* 引入方式：
1）下载js文件到本地，进行引入
<script src="jquery…js"></script>
* 复制代码
2）使用CDN（内容分发网络）
<script src="https://cdn."></script>
* 复制代码
第二种方式的优势：
1）在访问其他站点时，已经从CDN中加载过JQuery，访问的当前站点时可直接使用缓存，减少加载时间。
2）大多数的CDN都可以确保用户向其请求文件时，会从最近的服务器上返回响应，提高加载速度。
版本查询：$.fn.jquery
2. 基础知识点
* 语法
通过选取HTML元素，并对选取的元素执行某种操作。
$(selector).action()
$：代表JQuery
(selector)：查询和选取HTML元素
action()：执行对选取元素的操作

入口/文档就绪事件：
在html所有标签DOM都加载完后执行。
$(document).ready(function(){
//代码内容
复制代码
});
可简写为：
$(function(){
  //代码内容
复制代码
});
function()在action()执行完成后触发的。比如ready后，进行某种操作。click()点击后，进行日志打印之类的。
* AJAX
AJAX = 异步javascript和xml，Asynchronous Javascript And Xml
在不重载整个网页的情况下，AJAX通过后台加载数据，并在网页上显示。
load()方法实现
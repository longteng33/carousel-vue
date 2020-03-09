# carousel-vue
用vue动画写的轮播图<br>
https://longteng33.github.io/carousel-vue/<br>
1、此页面不是用vue-cli创建的，而是在html中通过script标签引用在线的vue.js文件
2、通过es6模块化语法，在throttle.js文件中暴露函数，export function throttle
3、通过es6语法，引入模块，<script type="module">，需要写上type，
 import {throttle} from "./throttle.js"
 4、为此轮播图的上下点击事件增加的节流函数处理，节流后点击效果并不怎么好

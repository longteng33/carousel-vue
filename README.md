# carousel-vue
用vue动画写的轮播图<br>
https://longteng33.github.io/carousel-vue/<br>
1、此页面不是用vue-cli创建的，而是在html中通过script标签引用在线的vue.js文件<br>
2、通过es6模块化语法，在throttle.js文件中暴露函数，export function throttle<br>
3、通过es6语法，引入模块，<script type="module">，需要写上type，<br>
 import {throttle} from "./throttle.js"<br>
 4、为此轮播图的上下点击事件增加的节流函数处理，节流后点击效果并不怎么好(就好像使劲点点不动一样)<br>
 
 5、使用vue做动画，是在条件渲染(v-if)、条件展示(v-show)、动态组件进行切换的时候有动画的xiaoguo<br>
 6、用transition标签包裹想要有动画的dom节点（智能包裹单个元素）<br>
 7、用transition-group标签包裹列表，实现列表的过度（多个元素）<br>
 8、实现动画的关键是为transition添加name属，在动画进入/离开的过程中，有6个类命的切换，它们是：<br>
 1)v-enter<br>
 2)v-enter-active<br>
 3)v-enter-to<br>
 4)v-leave<br>
 5)v-leave-active<br>
 6)v-leave-to<br>
<br>
 8、当transition标签没给name属性值时，这6个类名的默认前缀是v-<br>
 9、当给了transition标签name属性值时，这6个类名的前缀就是 “name的属性值-”<br>
 10、在v-enter-active、v-leave-active中使用transition或animation来实现动画效果<br>
 11、transition有8个钩子函数<br>
 12、animate.css是经典的动画库<br>

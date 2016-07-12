# myCssLib
常用css组件
这里的css组件主要指网站的常用组件，由于很多时候并没有必要完整引入bootstrap样式，这里的样式也是参考bootstrap样式，略其繁琐，取其样式精华。
最终目的是做到：1.能够随拿随用（复制粘贴），省去重复写常用样式的麻烦；2.稍微修改既能够获得索取样式

#Button
<pre>
   .btn-default{
                display: inline-block;
                padding: 6px 12px;
                background-color: #fff;
                /*border也可以设置0px*/
                /*不设置border-style，则按钮效果非常明显,具有立体感 左上与右下边框颜色不同*/
                border:1px solid #ccc;
                border-radius: 4px;
                outline: 0;

                /*btn 字体设置*/
                color: #333;
                letter-spacing: 1px;
                font-size: 14px;
                font-weight: 400;
                line-height: 1.42857143;
                white-space: nowrap;

                /*文本是否可以被选择*/
                -webkit-user-select: none;
                -moz-user-select: none;
                -ms-user-select: none;
                user-select: none;

                /*感觉没用的东西*/
                 margin-bottom: 0;
                 vertical-align: middle;
                 text-align:center;/*按钮本身文字能够实现上下左右居中*/
                 background-image: none;

                /*--不熟悉*/
                -ms-touch-action: manipulation;
                    touch-action: manipulation;
                    cursor: pointer;

                /*不清楚*/
                -webkit-box-sizing: border-box;
                -moz-box-sizing: border-box;
                box-sizing: border-box;
            }

            /*感觉没用*/
            .btn-default:after, .lib_button:before {
                -webkit-box-sizing: border-box;
                -moz-box-sizing: border-box;
                box-sizing: border-box;
            }

            .btn-default:hover {
                color: #333;
                background-color: #e6e6e6;
                border-color: #adadad;
            }
            /*点击时颜色是最深的*/
            .btn-default:active{
                color: #333;
                background-color: #e6e6e6;
                border-color: #adadad;
                background-image: none;
                -webkit-box-shadow: inset 0 3px 5px rgba(0,0,0,.125);
                box-shadow: inset 0 3px 5px rgba(0,0,0,.125);
            }
            /*获得焦点时的状态*/
            .btn-default:focus{
                color: #333;
                background-color: #e6e6e6;
                border-color: #8c8c8c;
            }
            /*以上三个伪类:完全模拟了button点击的一般效果，所以任何元素只要加上该类就能形成类似button的样式*/
</pre>
你好呀 <button class="btn-default">我是按钮</button><a class="lib_button">我是a标签按钮</a>

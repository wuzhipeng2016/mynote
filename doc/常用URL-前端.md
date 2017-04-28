backbone    http://www.css88.com/doc/backbone/
    backbone入门http://blog.csdn.net/joyhen/article/details/42528315
        http://blog.csdn.net/column/details/backbone-js-tutorial.html
        http://www.cnblogs.com/hiddenfox/archive/2012/08/19/2646429.html
mustache    http://www.cnblogs.com/yaozhenfa/p/js_mustache.html
lodash    https://lodash.com/docs
underscore http://www.css88.com/doc/underscore/
    最好的bindAll解释http://blog.bigbinary.com/2011/08/18/understanding-bind-and-bindall-in-backbone.html
requirejs    http://www.requirejs.cn/
zepto.js    http://www.css88.com/doc/zeptojs_api/
jquery    http://www.css88.com/jqapi-1.9/
jqueryUI    http://www.css88.com/jquery-ui-api/
css    http://www.css88.com/book/css/
html5    http://www.w3school.com.cn/html5/index.asp
echart    http://echarts.baidu.com/examples.html
jqwidgets    http://www.jqwidgets.com/jquery-widgets-documentation/
easyui    http://www.jeasyui.net/tutorial/index.html

jersey    http://www.tuicool.com/articles/IfUb6vb
    http://www.jdon.com/soa/jersey.html

easyui：http://www.jeasyui.com/download/index.php
2．文档：http://www.w3cschool.cc/jeasyui/jqueryeasyui-tutorial.html
3．部署：
1) 引用Jquery的Js文件<script src="jquery-easyui-1.3.4/jquery-1.8.0.min.js" type="text/javascript"></script>
2) 引用Easy UI的Js文件<script src="jquery-easyui-1.3.4/jquery.easyui.min.js" type="text/javascript"></script>
3) 导入Easy UI的主题Css文件<link href="jquery-easyui-1.3.4/themes/default/easyui.css" rel="stylesheet" type="text/css" />
4) 导入Easy UI的图标Css文件<link href="jquery-easyui-1.3.4/themes/icon.css" rel="stylesheet" type="text/css" />
5) 引用Easy UI的国际化文件以下为让它显示中文<script src="jquery-easyui-1.3.4/locale/easyui-lang-zh_CN.js" type="text/javascript"></script>
6) 页面上加上UTF-8编码       防止jquery.easyui.min.js  内容乱码
<meta http-equiv="content-type" content="text/html;charset=UTF-8" />

1st:
<script type="text/javascript" src="Js/2-1.js" ></script>
<link rel="stylesheet" type="text/css" href="Css/2-1.css">
2nd:
<script type="text/javascript">
alert("aa");
</script>
<style type="text/css">
:root{color:red;}
</style>
3rd:
匿名函数自运行
(function(msg){
    alert(msg);
})("hello");
4th:jquery
$(function(){
    alert("aa");
});

form json格式
http://marsvaadin.iteye.com/blog/1717188
(function($){
        $.fn.serializeJson=function(){
            var serializeObj={};
            $(this.serializeArray()).each(function(){
                serializeObj[this.name]=this.value;
            });
            return serializeObj;
        };
    })(jQuery);


(function($){
        $.fn.serializeJson=function(){
            var serializeObj={};
            var array=this.serializeArray();
            var str=this.serialize();
            $(array).each(function(){
                if(serializeObj[this.name]){
                    if($.isArray(serializeObj[this.name])){
                        serializeObj[this.name].push(this.value);
                    }else{
                        serializeObj[this.name]=[serializeObj[this.name],this.value];
                    }
                }else{
                    serializeObj[this.name]=this.value;    
                }
            });
            return serializeObj;
        };
    })(jQuery);


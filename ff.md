$(document).delegate('button','click',function () {
    alert($(this).html());   //$(this)访问添加事件的元素
});

var btn = document.createElement('button');
$(btn).html('hi');
$(btn).insertAfter('button')

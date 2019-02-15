$(document).delegate('button','click',function () {
    alert($(this).html());   //$(this)访问添加事件的元素
});

var btn = document.createElement('button');
$(btn).html('hi');
$(btn).insertAfter('button')




document.onclick = function(event){
    //IE doesn't pass in the event object
    event = event || window.event;
    //IE uses srcElement as the target
    var target = event.target || event.srcElement;
    target.onclick = function () {
        alert(target.innerHTML.substr(3));
    }
};

document.onclick = function(event)
this，表示当前的上下文对象是一个html DOM对象，可以调用html对象所拥有的属性，方法。
$(this),代表的上下文对象是一个jquery的上下文对象，可以调用jquery的方法和属性值。
		$(document).ready(function(){
          $('#out').mouseup(function(){
          	$(this).css("color","red");
          });
		});
   比如上例中的$(this)中的this就是指#out.

$("#img").attr("width","300")
$("#img").attr({"width":"300","height":"300"})
这个操作与jquery的css()操作类似,可以设置一个属性值,同时也可以设置多个属性值,设置多个时,是以对象的形式写的。
          $("#button2").mousedown(function(){
          	$("#wan").attr("title","坚果");
          	alert($("#wan").attr("title"));
          });
          $("#button").mouseenter(function(){
          	$("#wan2").attr("title",function(){return this.value});
          	alert($("#wan2").attr("title"));
          });
	  
查找每个段落的带有 "selected" 类的父元素：
$("p").parent(".selected")


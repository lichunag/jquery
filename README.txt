this，表示当前的上下文对象是一个html DOM对象，可以调用html对象所拥有的属性，方法。
$(this),代表的上下文对象是一个jquery的上下文对象，可以调用jquery的方法和属性值。
		$(document).ready(function(){
          $('#out').mouseup(function(){
          	$(this).css("color","red");
          });
		});
   比如上例中的$(this)中的this就是指#out.

jsonp:


<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
	</head>
	<body>
		<button>button</button>
			<div id="box"></div>
		<input type="text" />
	</body>
	<script> 
	         /*
		    jsonp同ajax都是获取数据
		 */
		  function fn(data){
		  	   console.log(data)
		  }
		  var btn=document.querySelector('button');
		  
		  btn.onclick=function(){
		  	 var sc=document.createElement('script');
		  	 sc.src='http://localhost:88/jsonp/1.js';
		  	 document.querySelector('body').appendChild(sc)
		  }
		  
	</script>
</html>

/ES6面向对象写法，用class类,如果使用class的方式写类，那么类的prototy是不能被赋值改写的
			
			//ES6继承
			/*
			    class 子类 extends 父类{
			    	constructor(name,age,..自己的属性){
			    		 super(name,age);
			    		 自己的属性添加，必须要放在super下边
			    	}
			    	sing(){
			    		自己的方法添加
			    	}
			    }

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


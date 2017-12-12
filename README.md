<!DOCTYPE html>
<html>
<head>
	<title>ss</title>
<style type="text/css">
#div1{
	
	width: 600px;
	height: 350px;
	background-color: red;
}
#div2{
	background-color: black;
	width: 80px;
	height: 80px;
	padding: 20px;
	position: relative;
	left:240px;
	top:105px;
}
</style>
<script type="text/javascript">
window.onload=function(){
	document.getElementById("btn1").onclick=function(){
		document.getElementById("btn1").style.background="radial-gradient(at top left,white,red)";
		document.getElementById("div2").style.boxShadow="10px 10px 10px yellow";
	}
	document.getElementById("btn2").onclick=function(){
		document.getElementById("div1").style.background="radial-gradient(at top left,white,red)";
		document.getElementById("div2").style.boxShadow="-10px 10px 10px yellow";
	}
	document.getElementById("btn3").onclick=function(){
		document.getElementById("div1").style.background="radial-gradient(at top left,white,red)";
		document.getElementById("div2").style.boxShadow="0px -10px 10px yellow";
	}
}
</script>
</head>
<body>
<div id="div1">
<div id="div2">
LIGHT:<br/>
<input type="button" id="btn1" value="Top Left"><br/>
<input type="button" id="btn2" value="Top Right"><br/>
<input type="button" id="btn3" value="Bottom"><br/>
</div>
</div>
</body>
</html>
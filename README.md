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




<!DOCTYPE html>
<html>
<head>
	<title>ssda</title>
	<style type="text/css">
     span{
     	font-size: 16pt;
     	font-family: arial,helvetica,sans-serif;
       padding: 20px;
     }
	</style>
	<script type="text/javascript">
      function toggle(){
         var myElement=document.getElementById("id1");
         if(myElement.style.backgroundColor=='red'){
         	myElement.style.backgroundColor='yellow';
         	myElement.style.color='white';
         }else{
         	myElement.style.backgroundColor='red';
         	myElement.style.color='white';
         }

      }
      window.onload=function(){
      	document.getElementById("btn1").onclick=toggle;
      }
	</script>
</head>
<body>
<span id="id1">dsaa sdas d a</span>
<input type="button" id="btn1" value="Toggle">
</body>
</html>







<!DOCTYPE html>
<html>
<head>
	<title></title>
	<script type="text/javascript">
       function myObjectType(){
       	  this.info='I am a shiny new object';
       	  this.showInfo=function(){
       	    alert(this.info);
       	  }
       	  this.setInfo=function (newInfo){
       	  	this.info=newInfo;
       	  }
       }
         var myNewObject1=new myObjectType();
         var myNewObject2=new myObjectType();
	</script>
</head>
<body>
<input type="button" value="show Info 1" onclick="myNewObject1.showInfo()"/>
<input type="button" value="show Info 2" onclick="myNewObject2.showInfo()"/>
<input type="button" value="Change info of object2" onclick="myNewObject2.setInfo('New Information!')"/>
</body>
</html>
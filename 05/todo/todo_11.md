﻿TODO 11
========

* 아래 sum() 함수를 구현해주세요.
* Math.max 함수 사용하지 마세요.
* Math.min 함수 사용하지 마세요.

```javascript
function sum() {
	var list = [["penny01",100,100,200,300,400],
				["penny02",90,100,200,300],
				["penny03",80,100,200,300,400,500],
				["penny04",70,100,200,300],
				["penny05",60,100,200,300,300],
				["penny06",50,100,200,200,200,200],
				["penny07",40,100,200],
				["penny08",30,100,200],
				["penny09",20,100,200,100,100,100],
				["penny10",10,100,200] ];

	//
	// TO DO : list 배열은 이름과 성적을 포함한 배열을 담고 있습니다. 
	// 1. 배열 list 에 성적만 빼내서 합산합니다.
	//    ( (100 + 100 + 200 + 300 + 400) + (90 + 100 + 200 + 300) ... + (10 + 100 + 200))
	// 2. 합산 결과를 리턴합니다.
}

```

> 초기 화면

![TODO11](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_11.png)


>  결과 화면

![TODO11](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_11_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum() {

				var list = [["penny01",100,100,200,300,400],
							["penny02",90,100,200,300],
							["penny03",80,100,200,300,400,500],
							["penny04",70,100,200,300],
							["penny05",60,100,200,300,300],
							["penny06",50,100,200,200,200,200],
							["penny07",40,100,200],
							["penny08",30,100,200],
							["penny09",20,100,200,100,100,100],
							["penny10",10,100,200] ];
													
			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum();
					document.getElementById("result").value = value;
					
				};
			}			
		</script>
	</head>
<body onload="init()">               
	<input type="button" id="calculation" value="calculation"/>        
	<input type="text" id="result"/> 
</body>
</html>

```

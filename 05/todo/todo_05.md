TODO 05
========

* 아래 sum() 함수를 구현해주세요.
* Math.max 함수 사용하지 마세요.
* Math.min 함수 사용하지 마세요.
* 배열 사용하지 마세요.

```javascript
function sum() {
	var a01 = 1;
	var a02 = 2;
	var a03 = 3;
	var a04 = 4;
	var a05 = 5;
	var a06 = 6;
	var a07 = 7;
	var a08 = 8;
	var a09 = 9;
	var a10 = 10;
	
	//
	// TO DO : 위에 선언한 변수값 중에서 최대값과 최소값을 제외한 나머지 값들의 합을 리턴하는 코드를 작성해주세요.
	//
}

```

> 초기 화면

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_05.png)


>  결과 화면

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_05_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum() {
				var a01 = 1;
				var a02 = 2;
				var a03 = 3;
				var a04 = 4;
				var a05 = 5;
				var a06 = 6;
				var a07 = 7;
				var a08 = 8;
				var a09 = 9;
				var a10 = 10;
				
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

TODO 05
========

* 아래 sum() 함수를 구현해주세요.

```javascript

function sum() {

	var a01 = 100;
	var a02 = "100";
	var a03 = [100, 200];
	var a04  = ["100", "200"];
	var a05 = [[100, 200]];
	var a06 = [["100", "200"]];
	var a07 = { score : 100};
	var a08 = { score : "100"};
	var a09 = { score : [100, 200]};
	var a10 = { score : ["100", "200"]};
	var a11 = function() { return 100; };
	var a12 = function() { return "100"; };
	var a13 = function() { return [100, 200];}
	var a14 = function() { return ["100", "200"];}
	var a15 = function() { return [["100", "200"]];};
	var a16 = function() { return { score : 100};};
	var a17 = function() { return { score : "100"};};
	var a18 = function() { return { score : [100, 200]};};
	var a19 = function() { return { score : ["100", "200"]};};
	var a20 = function() { return function() { return 100; };};
	var a21 = function() { return function() { return "100"; };};
	var a22 = function() { return function() { return [100, 200]; };};
	
	var sum = 0;

	//
	// TO DO : 변수 a01 ~ a22 의 값을 모두 합산한 결과를 리턴하는 함수를 작성해주세요.
	//         1. 배열 : 배열의 원소를 모두 합산해주세요(문자이면 숫자로 변환)
	//         2. 객체 : score  속성의 값을 합산주세요(문자이면 숫자로 변환)
	//         3. 함수 : 함수의 리턴 값을 합산해주세요(문자이면 숫자로 변환)   
	//	
	
	return sum;
	
}
			

```

> 초기 화면

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_05.png)


>  결과 화면

![TODO05](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_05_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum() {
			
				var a01 = 100;
				var a02 = "100";
				var a03 = [100, 200];
				var a04  = ["100", "200"];
				var a05 = [[100, 200]];
				var a06 = [["100", "200"]];
				var a07 = { score : 100};
				var a08 = { score : "100"};
				var a09 = { score : [100, 200]};
				var a10 = { score : ["100", "200"]};
				var a11 = function() { return 100; };
				var a12 = function() { return "100"; };
				var a13 = function() { return [100, 200];}
				var a14 = function() { return ["100", "200"];}
				var a15 = function() { return [["100", "200"]];};
				var a16 = function() { return { score : 100};};
				var a17 = function() { return { score : "100"};};
				var a18 = function() { return { score : [100, 200]};};
				var a19 = function() { return { score : ["100", "200"]};};
				var a20 = function() { return function() { return 100; };};
				var a21 = function() { return function() { return "100"; };};
				var a22 = function() { return function() { return [100, 200]; };};
				
				var sum = 0;

				
				return sum;
				
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

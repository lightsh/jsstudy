TODO 04
========

* 아래 sum() 함수를 구현해주세요.

```javascript

function sum(list) {
	
	//
	// TO DO : 인자 list 는 배열입니다. 배열에 있는 값들의 합을 리턴하는 함수를 작성해주세요.
	//
}

```

> 초기 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_04.png)


>  결과 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_04_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum(list) {

			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum([
					                   [1, 2, 3, 4, 5, 6, 7, 8, 9], 
									   [10, 11, 12, 13, 14, 15, 16, 17, 18], 
									   [19, 20]
									 ]);
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

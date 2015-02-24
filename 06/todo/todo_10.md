TODO 10
========

* 아래 sum() 함수를 구현해주세요.
* String.split() 함수를 사용하지 마세요.

```javascript

function sum(text) {

	//
	// TO DO : 인자 text 는 문자열입니다.
	// 문자열을 ","로 분리한 다음, 더한 값을 아래 형태의 문자로 리턴하는 함수를 작성해주세요.
	// text.split(",") 함수를 사용하지 마세용!!!
	//
	
}		

```

> 초기 화면

![TODO10](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_10.png)


>  결과 화면

![TODO10](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_10_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum(text) {

			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum("100, 200, 300, 400, 500, 600, 700, 800, 900");
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

TODO 02
========

* 아래 count() 함수를 구현해주세요.

```javascript
function count(text) {
	
	//
	// TO DO : 인자 text는 문자열입니다. 단어(word)의 개수를 리턴하는 함수를 작성해주세요.
	//        
}

```

> 초기 화면

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_02.png)


>  결과 화면

![TODO02](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_02_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">	
		</style>
		<script type="text/javascript">
			function count(text) {

			}
			
			function init() {
					document.getElementById("show").onclick = function() {
					var value = count("    JavaScript     is    the programming    language    of    the Web   ");
					document.getElementById("result").value = "The word count is " + value ;
					
				};
			}			
		</script>
	</head>
<body onload="init()">               
	<input type="button" id="show" value="Show the word count!"/>        
	<input type="text" id="result"/> 
</body>
</html>

```

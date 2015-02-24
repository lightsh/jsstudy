TODO 03
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

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_03.png)


>  결과 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_03_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">			
		textarea {
				width: 650px;
				height: 200px;		
			}			
		</style>
		<script type="text/javascript">
			function count(text) {

			}
			
			window.onload = function() {
					document.getElementById("show").onclick = function() {
					var value = count(document.getElementById("text").value);
					document.getElementById("result").value = "The word count is " + value ;
					
				};
			}			
		</script>
	</head>
<body> 
	<textarea id="text">JavaScript is the programming language of the Web.

All modern HTML pages are using JavaScript.

JavaScript is easy to learn.

This tutorial will teach you JavaScript from basic to advanced.</textarea><br>
	<input type="button" id="show" value="Show the word count!"/>        
	<input type="text" id="result"/> 
</body>
</html>

```

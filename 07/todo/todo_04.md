TODO 04
========

* 아래 count() 함수를 구현해주세요.
* 아래 display() 함수를 구현해주세요.

```javascript
function count(text) {
	
	//
	// TO DO : 인자 text는 문자열입니다. 
	//         1. 문자열에서 검색된 단어(word)를 배열에 담아 리턴하는 함수를 작성해주세요.
	//         2. 단어(word)를 검색할 때 특수 문자 콤마(.)는 제외하세요.
	//            예) Web. -> 틀림, Web -> 맞음
	//        
}


function display(list) {
	
	//
	// TO DO : 인자 list 는 문자열이 담긴 배열입니다. 
	//         1. 배열에 담긴 단어를 테이블로 보여주는 코드를 작성해주세요.
	//            1.1. 첫번째 열 NO 에는 0 번부터 차례대로 순번을 매겨 주세요.
	//            1.2. 두번째 열 Word 에는 단어를 표시해주세요.
	//         2. 테이블 id 는 "wordlist" 입니다.
	//        
}

```

> 초기 화면

![TODO04](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_04.png)


>  결과 화면

![TODO04](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_04_result.png)

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
			
			function display(list) {
					
			}
			
			window.onload = function() {
					document.getElementById("show").onclick = function() {
					var words = count(document.getElementById("text").value);
					document.getElementById("result").value = "The word count is " + words.length ;
					display(words);
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
	<table id="wordlist" border="1">
		<tr> 
			<th width="150px">No</th>
			<th width="150px">Word</th>
		</tr>	
	</table> 
</body>
</html>

```

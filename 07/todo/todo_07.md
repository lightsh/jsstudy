TODO 07
========

* 아래 count() 함수를 구현해주세요.
* 아래 display() 함수를 구현해주세요.

```javascript
function count(text) {
	
	//
	// TO DO : 인자 text는 문자열입니다. 
	//         1. 문자열에서 검색된 단어(word)와 중복 개수를  배열에 담아 리턴하는 함수를 작성해주세요.
	//         2. 단어(word)를 검색할 때 아래 특수 문자를 제외하세요.
	//            '.',  ':',  '(' . ')', '"', '!', ','
	//            예) Web. -> 틀림, Web -> 맞음
	//                (the -> 틀림, the -> 맞음
	//                Yourself". -> 틀림, Yourself -> 맞음
	//         3. 중복된 단어(word)는 배열에 추가 하지 마세요. 대신 중복 개수를 증가 시켜 주세요.
	//         4. 쌍따옴표(" ~ ") 로 묶인 문자열은 한 문자로 처리해주세요.
	//            예) "Try it Yourself" -> 'Try it Yourself'를 한 단어로 취급
	//         5. 괄호("( ~ )") 로 묶인 문자열은 한 문자로 처리해주세요.
	//            예) (the Document Object Model) -> 'the Document Object Model'를 한 단어로 취급 
}


function display(list) {
	
	//
	// TO DO : 인자 list 는 문자열이 담긴 배열입니다. 
	//         1. 배열에 담긴 단어를 테이블로 보여주는 코드를 작성해주세요.
	//            1.1. 첫번째 열 NO 에는 0 번부터 차례대로 순번을 매겨 주세요.
	//            1.2. 두번째 열 Word 에는 단어를 표시해주세요.
	//            1.3. 세번째 열 Count 에는 중복 개수를 표시해주세요.
	//         2. 테이블 id 는 "wordlist" 입니다.
	//        
}

```

> 초기 화면

![TODO07](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_07.png)


>  결과 화면

![TODO07](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_07_result.png)

![TODO07](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_07_result2.png)

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
	<textarea id="text">JavaScript is one of 3 languages all web developers must learn:

This tutorial contains hundreds of examples!

All examples are "Try it Yourself".

You can edit every example online, and view the result directly.

The HTML DOM (the Document Object Model) is the official W3C standard for accessing HTML elements.

JavaScript can manipulate the DOM (change HTML contents).</textarea><br>
	<input type="button" id="show" value="Show the word count!"/>        
	<input type="text" id="result"/>
	<table id="wordlist" border="1">
		<tr> 
			<th width="150px">No</th>
			<th width="150px">Word</th>
			<th width="150px">Count</th>
		</tr>	
	</table> 
</body>
</html>

```

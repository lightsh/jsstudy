﻿TODO 03
========

* 아래 sum() 함수를 구현해주세요.

```javascript

function sum(listA, listB, listC) {

	//
	// TO DO : 인자 listA, listB, listC 는 배열입니다. 
	// 배열 listA, listB, listC 에 있는 값들의 합을 리턴하는 함수를 작성해주세요.
	//
}

```

> 초기 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_03.png)


>  결과 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_03_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum(listA, listB, listC) {

			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum([1, 2, 3, 4, 5, 6, 7, 8, 9], [1, 2, 3, 4, 5, 6, 7, 8, 9], [100, 200, 300]);
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
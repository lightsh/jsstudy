TODO 06
========

* 아래 maximum() 함수를 구현해주세요.

```javascript

function maximum(listA, listB) {

	//
	// TO DO : 인자 listA, listB 는 배열입니다. 
	// 두 배열에서 가장 큰 값을 리턴하는 함수를 작성해주세요.
	//
	
}		

```

> 초기 화면

![TODO06](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_06.png)


>  결과 화면

![TODO06](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/06/todo/images/todo_06_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function maximum(listA, listB) {

			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = maximum([1, 2, 3, 4, 5, 6, 7, 8, 9], [10, 11, 12, 13, 14, 15, 16, 17, 18, 19]);
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

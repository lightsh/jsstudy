TODO 07
========

* 아래 maximum_sum() 함수를 구현해주세요.

```javascript

function maximum_sum(list) {

	//
	// TO DO : 인자 list는 2차원 배열입니다. 
	// 각 배열의 가장 큰 값(max)을 더한 값을 리턴하는 함수를 작성해주세요.
	// return list[0]의 max  + list[1]의 max ~  list[n]의 max
	//
	
}		

```

> 초기 화면

![TODO07](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_07.png)


>  결과 화면

![TODO07](https://raw.githubusercontent.com/lightsh/jsstudy/master/06/todo/images/todo_07_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function maximum_sum(list) {

			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = maximum_sum([ [1, 2, 3, 4, 5, 6, 7, 8, 9], 
					                          [10, 11, 12, 13, 14, 15, 16, 17, 18, 19], 
											  [100, 200, 300],
											  [1000, 2000, 3000],
											  [10000, 20000, 30000]
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

TODO 02
========

* 아래 return_sum_array(), sum() 함수를 구현해주세요.


```javascript

function return_sum_array(arrayA, arrayB) {

	//
	// TO DO : 인자 arrayA, arrayB 은 숫자를 담은 배열입니다.
	//         1. 배열 arrayA, arrayB의 사이즈는 다를 수 있습니다!!!!
	//         2. 배열 arrayA 와 배열 arrayB의 값을 더한 결과를 배열로 리턴 합니다.
	//            예)  arrayA = [1, 2, 3, 4, 5, 6, 7]
	//                 arrayB = [5, 6, 7, 8]
	//                 arrayA 와 arrayB 의 값이 위와 같을 경우 [6, 8, 10, 12, 5, 6, 7] 을 리턴합니다.
	//         3. 배열의 사이즈가 다르면 큰 배열에 맞게 값을 더합니다.
	// 
	
}

function sum(array) {

	//
	// TO DO : 인자 array는 숫자를 담은 배열입니다.
	//         1. 배열 array에 담긴 숫자를 모두 더한 결과를 리턴합니다.
	// 
	
}

```

> 초기 화면

![TODO02](https://raw.githubusercontent.com/lightsh/jsstudy/master/09/todo/images/todo_02.png)


>  결과 화면

![TODO02](https://raw.githubusercontent.com/lightsh/jsstudy/master/09/todo/images/todo_02_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
			textarea {
				width : 200px;
				height : 200px;
			}
		</style>
		<script type="text/javascript">
		
			function return_sum_array(arrayA, arrayB) {

			}
			
			function sum(array) {

			}
			
			window.onload = function() {
			
					document.getElementById("calculation").onclick = function() {
							
					var result = return_sum_array([100, 100, 200, 300, 900, 600], [200, 300, 400, 500]);
					
					document.getElementById("result").value = sum(result);
				};
			}			
		</script>
	</head>
<body>               
	<input type="button" id="calculation" value="calculation"/>
    <br>	
    <textarea id="result">
	</textarea>
</body>
</html>

```

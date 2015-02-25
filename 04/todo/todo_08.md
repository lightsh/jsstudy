TODO 08
========

* N1, N2 값을 입력받아 sum한 결과를 RESULT에 보여주는 HTML을 작성해주세요.
* N1, N2 값으로 숫자만 입력한다고 전제합니다.
* sum 함수의 인자로 문자열이 들어갈 수 있습니다.
* sum 함수의 인자로 배열이 들어갈 수 있습니다.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript에서 sum() 함수만 작성해주세요.

```javascript

function sum() {
	//
	// TD DO : 여기에 함수를 구현해주세요.
	//				
}

```
			
> 초기 화면

![TODO08](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_08.png)


> 결과 화면

![TODO08](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_08_result.png)

## HTML template

```html
<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
		
			function sum() {
				//
				// TD DO : 여기에 함수를 구현해주세요.
				//	
			}
				
			window.onload = function() {
					document.getElementById("calculation").onclick = function() {
						//
						// TD DO : n1, n2 의 값을 얻어오는 코드를 작성해주세요.
						//	
						var value = sum(n1, n2);
						document.getElementById("result").value = value;
				};
			}			
		</script>
	</head>
<body>
	<table border="1">
		<tr>
			<td>N1</td>
			<td></td>
			<td>N2</td>
			<td></td>
			<td>RESULT</td>
		<tr>
		<tr>
			<td><input type="text" id="n1"/> </td>
			<td>+</td>
			<td><input type="text" id="n2"/> </td>
			<td><input type="button" id="calculation" value="="/></td>
			<td><input type="text" id="result"/>  </td>
		<tr>
	</table>   	
</body>
</html>

```

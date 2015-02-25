TODO 06
========

* "calculation" 버튼을 누르면 sum(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20)을 계산한 결과 값 210을 <input> 박스에 찍어주세요.
* sum 함수의 인자로 문자열이 들어갈 수 있습니다.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript에서 sum() 함수만 작성해주세요.

```javascript

function sum() {
	//
	// TD DO : 여기에 함수를 구현해주세요.
	//				
}

```
			
> 초기 화면

![TODO06](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_06.png)


> 결과 화면

![TODO06](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_06_result.png)

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
						var value = sum(1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20);
						document.getElementById("result").value = value;
				};
			}			
		</script>
	</head>
<body>               
	<input type="button" id="calculation" value="calculation"/> 
	<input type="text" id="result"/>      	
</body>
</html>

```

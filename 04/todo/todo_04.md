TODO 04
========

* "calculation" 버튼을 누르면 sum(1, 2, 3) + sum(4, 5) + sum(6) 을 계산한 결과 값 21을 <input> 박스에 찍어주세요.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript에서 sum(n1, n2, n3) 함수만 작성해주세요.

```javascript

function sum(n1, n2, n3) {
	//
	// TD DO : 여기에 함수를 구현해주세요.
	//				
}

```
			
> 초기 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_04.png)


> 결과 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/04/todo/images/todo_04_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum(n1, n2, n3) {
				//
				// TD DO : 여기에 함수를 구현해주세요.
				//	
			}
			
			window.onload = function() {
					document.getElementById("calculation").onclick = function() {
						var value = sum(1, 2, 3) + sum(4, 5) + sum(6);
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

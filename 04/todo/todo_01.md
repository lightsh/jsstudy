TODO 01
========

* "calculation" 버튼을 누르면 sum(1, 2) 을 계산한 결과 값을 alert 로 찍어주세요.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript에서 sum(n1, n2) 함수만 작성해주세요.

```javascript
function sum(n1, n2) {
	//
	// TD DO : 여기에 함수를 구현해주세요.
	//
}

```

> 초기 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/04/todo/images/todo_01.png)


>  결과 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/04/todo/images/todo_01_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum(n1, n2) {
			    //
				// TD DO : 여기에 함수를 구현해주세요.
				//
			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
						var value = sum(1, 2);
						alert(value);
				};
			}			
		</script>
	</head>
<body onload="init()">               
	<input type="button" id="calculation" value="calculation"/>        
</body>
</html>

```

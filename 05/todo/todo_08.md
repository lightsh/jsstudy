TODO 08
========

* 아래 sum() 함수를 구현해주세요.
* Math.max 함수 사용하지 마세요.
* Math.min 함수 사용하지 마세요.

```javascript
function sum() {
	var list = ["penny01,100", 
				"penny02,90",
				"penny03,80",
				"penny04,70",
				"penny05,60",
				"penny06,50",
				"penny07,40",
				"penny08,30",
				"penny09,20",
				"penny10,10" ];
		
	//
	// TO DO : 배열에는 문자열이 들어 있고 콤마(,)로 이름과 성적을 구분합니다. 
	// 1. 배열 list 에 성적만 빼내서 합산합니다.
	//    (100 + 90 + ... + 10)
	// 2. 합산 결과를 리턴합니다.
}

```

> 초기 화면

![TODO08](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/05/todo/images/todo_08.png)


>  결과 화면

![TODO08](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/05/todo/images/todo_08_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		</style>
		<script type="text/javascript">
			function sum() {

				var list = ["penny01,100", 
				            "penny02,90",
							"penny03,80",
							"penny04,70",
							"penny05,60",
							"penny06,50",
							"penny07,40",
							"penny08,30",
							"penny09,20",
							"penny10,10" ];
				
			}
			
			function init() {
					document.getElementById("calculation").onclick = function() {
					var value = sum();
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

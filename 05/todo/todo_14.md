TODO 14
========

* 아래 sum() 함수를 구현해주세요.
* Math.max 함수 사용하지 마세요.
* Math.min 함수 사용하지 마세요.

```javascript
function sum() {
	var list = ["penny01,100", 
				"penny01,90",
				"penny01,80",
				"penny01,70",
				"penny02,60",
				"penny02,50",
				"penny02,40",
				"penny01,30",
				"penny01,20",
				"penny02,10" ];

	//
	// TO DO : list 배열은 이름과 성적을 포함한 문자열을 담고 있습니다. 
	// 1. list 배열 안에는 동일한 이름이 있습니다. 동일한 이름 별로 합산을 계산해주세요.(최대값과 최소값은 제외)
	//    penny01 : 90 + 70 + 30(최대값 100, 최소값 20 제외)
	//    penny02 : 60 + 50 + 40 + 10(최대값 60, 최소값 10 제외)
	//
	// 2. 아래처럼 문자열을 리턴합니다.
	//  
	//   penny01  ----------> 270 points
	//   penny02  ----------> 90 points
	//
}

```

> 초기 화면

![TODO14](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_14.png)


>  결과 화면

![TODO14](https://raw.githubusercontent.com/lightsh/jsstudy/master/05/todo/images/todo_14_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
			textarea {
				width : 300px;
				height : 100px;
			}
		</style>
		<script type="text/javascript">
			function sum() {

				var list = ["penny01,100", 
				            "penny01,90",
							"penny01,80",
							"penny01,70",
							"penny02,60",
							"penny02,50",
							"penny02,40",
							"penny01,30",
							"penny01,20",
							"penny02,10" ];
				
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
	<br>
	<textarea id="result"></textarea> 
</body>
</html>

```

TODO 01
========

* 아래 cal() 함수를 구현해주세요.

```javascript
function cal(list) {
	
	//
	// TO DO : 인자 list 는 객체(학생 이름과 성적을 포함)를 담은 배열입니다. 
	//         1. 학생별로 성적의 합을(최대값과 최소값을 뺀) 계산합니다.
	//         2. 1단계에서 계산한 성적 합계를 모두 더한 결과를 리턴해주세요.
	//       
    //         penny01 is (110 - 50 - 10 ) = 50 
	//         penny02 is (220 - 90 - 20 ) = 110
	//         penny03 is (240 - 90 - 20 ) = 130
	//         penny04 is (190 - 80 - 20 ) = 90
	//         penny05 is (160 - 70 - 10 ) = 80
	//         penny06 is (260 - 80 - 50 ) = 130
	//         penny07 is (170 - 90 - 10 ) = 70
	//         penny08 is (170 - 90 - 20 ) = 60
	//         penny09 is (140 - 60 - 10 ) = 70
	//         penny10 is (160 - 80 - 10 ) = 70
	//         -----------------------------------
	//                                       860
	
}

```

> 초기 화면

![TODO01](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01.png)


>  결과 화면

![TODO01](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01_result.png)

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
		
			function cal(list) {
			
			}
			
			window.onload = function() {
			
					document.getElementById("calculation").onclick = function() {
					
					var penny01 = {"name" : "penny01", "score" : [10, 20, 30, 50]};
					var penny02 = {"name" : "penny02", "score" : [90, 60, 50, 20]};
					var penny03 = {"name" : "penny03", "score" : [20, 90, 50, 80]};
					var penny04 = {"name" : "penny04", "score" : [20, 40, 50, 80]};
					var penny05 = {"name" : "penny05", "score" : [10, 60, 20, 70]};
					var penny06 = {"name" : "penny06", "score" : [80, 70, 60, 50]};
					var penny07 = {"name" : "penny07", "score" : [10, 30, 40, 90]};
					var penny08 = {"name" : "penny08", "score" : [20, 20, 90, 40]};
					var penny09 = {"name" : "penny09", "score" : [60, 50, 20, 10]};
					var penny10 = {"name" : "penny10", "score" : [50, 10, 80, 20]};
					
					var value = cal([penny01, penny02, penny03, penny04, penny05, penny06, penny07, penny08, penny09, penny10]);
					document.getElementById("result").value = value;
					
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

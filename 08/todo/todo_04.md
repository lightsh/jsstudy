﻿TODO 04
========

* 아래 구현한 cal() 함수를 직접 코딩해보세요.
* 복사-붙여넣기 내공을 사용하지 마세요.
* 코딩은 머리가 아니라 손이 기억해요.
* 배열의 원소를 탐색할 때 forEach 함수를 사용해보세요.
* 2중 for 문을 없애 보세요. 
* 함수를 만들어 보세요.

```javascript
function sum(list) {
			
	var sum = 0;
	var max = list[0];
	var min = list[0];
	
	list.forEach(function(score) {
		sum += score;
		max = (max < score) ? score : max;
		min = (min > score) ? score : min;						

	});
	
	return (sum - max - min);
}

function cal(list) {

	var total = 0;				
	for(var i = 0; i < list.length; i++) {
		var student = list[i];
		var scores = student.score;
		total += sum(scores);
	}
	
	return total;
}

```

> 초기 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01.png)


>  결과 화면

![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01_result.png)

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

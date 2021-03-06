﻿TODO 08
========

* 아래 구현한 cal() 함수를 직접 코딩해보세요.
* 복사-붙여넣기 내공을 사용하지 마세요.
* 코딩은 머리가 아니라 손이 기억해요.
* 객체를 만들어 보세요.

```javascript

	
//
// 학생을 표현하는 객체(클래스) 입니다.
// 객체를 나타내는 경우 이름을 대문자로 시작합니다.(코딩 규약)
//
function Student(student) {				
	this.student = student;	

	//
	// Student 클래스에 sum 을 계산하는 추가합니다.
	//
	this.sum = function() {
		var sum = 0;
		this.student.score.forEach(function(score) {
			sum += score;					
		});					
		return sum;			
	};
	
	//
	// Student 클래스에 max 을 계산하는 추가합니다.
	//			
	this.max = function() {
			var max = this.student.score[0];
			this.student.score.forEach(function(score) {
				max = (max < score) ? score : max; 					
			});					
			return max;				
	}
	
	//
	// Student 클래스에 min 을 계산하는 추가합니다.
	//			
	this.min = function() {
		var min = this.student.score[0];
		this.student.score.forEach(function(score) {
			min = (min > score) ? score : min;			
		});					
		return min;			
	}				
	
}
			
function cal(list) {
	
	var total = 0;
	var students = [];
	//
	// Student 객체로 배열을 생성합니다.
	//
	for(var i = 0 ; i < list.length ; i++) {
		//
		// new 을 사용해서 객체를 생성합니다.
		//
		students.push(new Student(list[i]));
	}

	
	//
	// Student 객체를 탐색하면서 합계를 계산합니다.
	//				
	for(var i = 0 ; i < students.length ; i++) {
		var student = students[i];
		total += student.sum() - student.max() - student.min();
	}
	
	return total;
}



```

> 초기 화면

![TODO08](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01.png)


>  결과 화면

![TODO08](https://raw.githubusercontent.com/lightsh/jsstudy/master/08/todo/images/todo_01_result.png)

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

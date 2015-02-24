TODO 05
========

* 아래 merge_students(), print_students() 함수를 구현해주세요.


```javascript

function merge_students(students) {

	//
	// TO DO : 인자 students 은 객체를 담은 배열입니다.
	//         1.배열에 담긴 객체 중에서 동일한 이름(name)을 찾아서 성적(scorearray)을 머지(merge) 해주세요.
	//         예) {"name" : "penny01", "scorearray" : [100, 100, 200, 200]};
	//             {"name" : "penny01", "scorearray" : [200, 200, 100, 100]};
	//
	//          -> {"name" : "penny01", "scorearray" : [300, 300, 300, 300]};
	//
	//         2. 머지한 결과를 배열로 리턴해주세요.(인자 students 넘어온 객체와 동일한 형태)

	
}


function print_students(students) {

	//
	// TO DO : 인자 students 은 객체를 담은 배열입니다.
	//         1.배열을 루핑 돌면서 학생 단위로 아래와 같은 문자열을 만들어 리턴합니다.
	//           - {이름#1}의 평균은 {평균#1} 입니다."
	//           - {이름#2}의 평균은 {평균#2} 입니다."
	//           - {이름#2}의 평균은 {평균#3} 입니다."
	//         2. 객체의 scorearray 의 값을 사용하여 평균을 계산하는데 아래와 같은 조건이 있습니다.
	//           - 중복된 값은 제외하고 평균을 계산해주세요.
	//             예) [100, 100, 200, 300] 이면 평균은 (200 + 300) / 2 됩니다.
}


```

> 초기 화면

![TODO05](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/09/todo/images/todo_05.png)


>  결과 화면

![TODO05](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/09/todo/images/todo_05_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
			textarea {
				width : 200px;
				height : 200px;
			}
		</style>
		<script type="text/javascript">
		
			function merge_students(students) {

			}
			
			
			function print_students(students) {
			
			}

			
			window.onload = function() {
			
					document.getElementById("calculation").onclick = function() {
							
					var penny01 = {"name" : "penny01", "scorearray" : [100, 100, 200, 200]};
					var penny02 = {"name" : "penny02", "scorearray" : [100, 100, 100, 100]};
					var penny03 = {"name" : "penny03", "scorearray" : [100, 100, 100, 200]};
					var penny04 = {"name" : "penny04", "scorearray" : [100, 200, 300, 400]};
					var penny05 = {"name" : "penny01", "scorearray" : [200, 200, 200, 200]};
					var penny06 = {"name" : "penny02", "scorearray" : [200, 100, 100, 100]};
					var penny07 = {"name" : "penny03", "scorearray" : [200, 100, 100, 200]};
					var penny08 = {"name" : "penny04", "scorearray" : [200, 200, 300, 400]};
					
					
					var students = merge_students([penny01, penny02, penny03, penny04, penny05, penny06, penny07, penny08]);
					
					document.getElementById("result").value = print_students(students);
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

TODO 01
========

* 아래 cal() 함수를 구현해주세요.

```javascript
function cal(list) {
	
	//
	// TO DO : 인자 list 는 배열입니다. 배열의 내용을 아래와 같은 형태의 문자열을 리턴하는 함수를 작성해주세요.
	//        
	// penny01 : 10  20  30  50   sum : 110 max : 50 min : 10
	// penny02 : 90  60  50  20   sum : 220 max : 90 min : 20
	// penny03 : 20  90  50  80   sum : 240 max : 90 min : 20
	// penny04 : 20  40  50  80   sum : 190 max : 80 min : 20
	// penny05 : 10  60  20  70   sum : 160 max : 70 min : 10
	// penny06 : 80  70  60  50   sum : 260 max : 80 min : 50
	// penny07 : 10  30  40  90   sum : 170 max : 90 min : 10
	// penny08 : 20  20  90  40   sum : 170 max : 90 min : 20
	// penny09 : 60  50  20  10   sum : 140 max : 60 min : 10
	// penny10 : 50  10  80  20   sum : 160 max : 80 min : 10
	// ---------------------------------------------------------
	// sum     : 370 450 490 510 sum : 1820 max : 780 min : 180
	// max     : 90 90 90 90 sum : 260 max : 90 min : 50
	// min     : 10 10 20 10 sum : 110 max : 50 min : 10
	//
}

```

> 초기 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_01.png)


>  결과 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/07/todo/images/todo_01_result.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
			textarea {
				width : 400px;
				height : 400px;
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

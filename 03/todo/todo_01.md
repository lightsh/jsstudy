﻿TODO 01
========

* 두 개 테이블이 있습니다. 위쪽 테이블은 입력 부분이며, 아래쪽 목록 부분입니다. 입력 테이블에서 이름, 과목, 점수를 입력한 다음 "add" 버튼을 누르면 해당 내용을 아래 테이블에 추가합니다.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript 만 작성해주세요


> 초기 화면

![TODO01](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_01.png)


> 입력 후 화면

![TODO01](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_01_result.png)

## HTML template

```html
<!DOCTYPE html> 
<html>
	<head>
		<style type="text/css">
		
			/* 입력 테이블에 대한 CSS */
			table.input {
				font-family: verdana,arial,sans-serif;
				font-size:11px;
				color:#333333;
				border-width: 1px;
				border-color: #666666;
				border-collapse: collapse;				
			}
			
			table.input th {
				border-width: 1px;
				padding: 8px;
				border-style: solid;
				border-color: #666666;
				background-color: #dedede;				
			}
			
			table.input td {
				border-width: 1px;
				padding: 0px;
				border-style: solid;
				border-color: #666666;
				background-color: #ffffff;
				text-align: center;
			}	
			
			table.input input {
				width : 150px;
			}	
			
			/* 추가 버튼에 대한 CSS */
			table.input .add-button {
				color: #fff;
				background-color: rgb( 51, 102, 204 );
				border: 1px solid rgb( 44, 91, 104 );	
				text-decoration: none;
				text-shadow: 0 1px 1px rgba(0, 0, 0, 0.075);				
			}
			
			/* 성적 테이블에 대한 CSS */
			table.reportcard {
				font-family: verdana,arial,sans-serif;
				font-size:11px;
				color:#333333;
				border-width: 1px;
				border-color: #666666;
				border-collapse: collapse;				
			}
			
			table.reportcard th {
				border-width: 1px;
				padding: 8px;
				border-style: solid;
				border-color: #666666;
				background-color: #dedede;				
			}
			
			table.reportcard td {
				border-width: 1px;
				padding: 8px;
				border-style: solid;
				border-color: #666666;
				background-color: #ffffff;
			}	
				
		</style>
		<script type="text/javascript">		
		
		</script>
	</head>
<body>               
	<table class="input">
		<tr> 
			<th width="150px">Name</th>
			<th width="150px">Subject</th>
			<th width="150px">Score</th>
			<th width="150px"></th>
		</tr>
		<tr> 
			<td><input type="text" id="name"></td>
			<td><input type="text" id="subject"></td>
			<td><input type="text" id="score"></td>
			<td><input type="button" class="add-button" id="add-button" value="add"></td>
		</tr>		
	</table> 
	<p/>
	<table class="reportcard" id="reportcard">
		<tr> 
			<th width="150px">No</th>
			<th width="150px">Name</th>
			<th width="150px">Subject</th>
			<th width="150px">Score</th>
		</tr>	
	</table> 
</body>
</html>
```
> 참고

Javascript로 테이블에 행을 추가하는 방법은 아래 사이트를 참고하세요. [http://www.w3schools.com/jsref/met_table_insertrow.asp](http://www.w3schools.com/jsref/met_table_insertrow.asp) 


```javascript
// Find a <table> element with id="myTable":
var table = document.getElementById("myTable");

// Create an empty <tr> element and add it to the 1st position of the table:
var row = table.insertRow(0);

// Insert new cells (<td> elements) at the 1st and 2nd position of the "new" <tr> element:
var cell1 = row.insertCell(0);
var cell2 = row.insertCell(1);

// Add some text to the new cells:
cell1.innerHTML = "NEW CELL1";
cell2.innerHTML = "NEW CELL2";

```

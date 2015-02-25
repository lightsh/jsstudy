TODO 02
========

* 아래쪽 테이블에 삭제 버튼(delete)을 추가해주세요.
* 삭제 버튼(delete)을 클릭하면 해당 성적을 삭제해주세요.(테이블에서 행을 삭제해야 합니다)
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript 만 작성해주세요.


> 초기 화면

![TODO02](https://github.com/lightsh/jsstudy/blob/master/javascript/03/todo/images/todo_02.png)


> 삭제 후 화면

![TODO02](https://github.com/lightsh/jsstudy/blob/master/javascript/03/todo/images/todo_02_result.png)

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
			
			table.reportcard input {
				width : 150px;
			}	
			
			/* 삭제 버튼에 대한 CSS */
			table.reportcard .delete-button {
				width: 50px;
				color: #fff;
				background-color: rgb( 207, 56, 91 );
				border: 1px solid rgb( 187, 40, 74 );
				text-decoration: none;
				text-shadow: 0 1px 1px rgba(0, 0, 0, 0.075);				
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
			<th width="50px">Delete</th>
		</tr>	
	</table>
</body>
</html>
```

> 참고

Javascript로 테이블에 행을 삭제하는 방법은 아래 사이트를 참고하세요. [http://www.w3schools.com/jsref/met_table_deleterow.asp](http://www.w3schools.com/jsref/met_table_deleterow.asp) 


```javascript
function deleteRow(r)
{
var i = r.parentNode.parentNode.rowIndex;
document.getElementById("myTable").deleteRow(i);
}

```

```javascript
function myCreateFunction()
{
var table = document.getElementById("myTable");
  {
  var row = table.insertRow(0);
  var cell1 = row.insertCell(0);
  var cell2 = row.insertCell(1);
  cell1.innerHTML = "NEW CELL1";
  cell2.innerHTML = "NEW CELL2";
  }
}
function myDeleteFunction()
{
document.getElementById("myTable").deleteRow(0);
}

```

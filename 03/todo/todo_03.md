TODO 03
========

* 아래쪽 테이블에 편집 버튼(edit)을 추가해주세요.
* 편집 버튼(edit)을 클릭하면 입력한 내용(이름, 과목, 성적)을 편집할 수 있게 각 셀에 입력(input) 박스를 보여주세요.
* 편집 버튼(edit)을 클릭하면 버튼의 타이틀을 "done" 으로 변경해주세요.
* 편집 상태에서 편집 버튼(edit)을 클릭하면 변경된 내용을 셀에 반영하고 버튼의 타이틀을 원래대로 "edit"로 변경해주세요.
* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript 만 작성해주세요.
* 편집 버튼(edit)의 class로 "edit-button"을 사용해주세요.

> 초기 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/03/todo/images/todo_03.png)


> 편집 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/03/todo/images/todo_03_edit.png)


> 편집을 마친 후 화면

![TODO03](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/03/todo/images/todo_03_result.png)

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
				color: #fff;
				background-color: rgb( 43, 153, 91 );
				border: 1px solid rgb( 33, 126, 74 );				
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
				
			/* 변경 버튼에 대한 CSS */
			table.reportcard .edit-button {
				width: 50px;
				color: #fff;
				background-color: rgb( 43, 153, 91 );
				border: 1px solid rgb( 33, 126, 74 );
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
			<th width="50px">Edit</th>
		</tr>	
	</table>
</body>
</html>
```

> 참고

Javascript로 input 태그를 생성하는 방법은 아래 사이트를 참고하세요. 
[http://www.w3schools.com/jsref/dom_obj_text.asp](http://www.w3schools.com/jsref/dom_obj_text.asp) 


```javascript

function myFunction() {
    var x = document.createElement("INPUT");
    x.setAttribute("type", "text");
    x.setAttribute("value", "Hello World!");
    document.body.appendChild(x);
}

```


﻿TODO 09
========

* 아래쪽 테이블에 성적(score)에 대한 필터를 추가해주세요.
* 필터에서 선택한 점수 이상만 테이블에 보여주세요.
* 필터가 "all" 이면 모든 목록을 보여주세요.
* 필터를 적용해서 평균도 업데이트해주세요.


filter | description
------------  | ------------ 
all  | 모든 성적
90+  | 90점 이상
80+  | 80점 이상
70+  | 70점 이상
60+  | 60점 이상
50+  | 50점 이상
40+  | 40점 이상
30+  | 30점 이상
20+  | 20점 이상
10+  | 10점 이상

* HTML의 모양새는 아래 HTML template을 사용하고 JavaScript 만 작성해주세요.


> 초기 화면

![TODO09](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_09.png)


> 필터 선택 화면

![TODO09](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_09_filter.png)


> 필터로 `50`을 선택한 화면

![TODO09](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_09_filter_50.png)


> 필터로 `20`을 선택한 화면

![TODO09](https://raw.githubusercontent.com/lightsh/jsstudy/master/03/todo/images/todo_09_filter_20.png)

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
			
			table.input input, table.input select{
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
			
			table.reportcard input, table.reportcard select {
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
			
			
			/* 선택된 행을 하이라이트 시키기 위한 CSS */
			table.reportcard tr:hover td, table.reportcard tr:hover input, table.reportcard tr:hover select{
				background:rgba(41,137,216, 0.75);
				border:1px solid #1E5799;
			}
		
			
			/* 평균에 대한 CSS */
			table.reportcard .average {
				font-family: verdana,arial,sans-serif;
				font-size:20px;
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
			<td>
				<select id="subject">
					<option value="javascript">javascript</option>
					<option value="html">html</option>
					<option value="c++">c++</option>
					<option value="java">java</option>
					<option value="python">python</option>
					<option value="perl">perl</option>
					<option value="ruby">ruby</option>
					<option value="closure">closure</option>
				</select>
			</td>
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
		<tr> 
			<td></th>
			<td></th>
			<td></th>
			<td class = "average "id="average">0</th>
			<td></th>
			<td></th>
		</tr>		
	</table>  
</body>
</html>
```





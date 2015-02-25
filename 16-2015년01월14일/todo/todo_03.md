TODO 03
========

* TODO 02 에서 만든 코드를 jQuery를 사용해서 다시 만들어 보세요.
* TODO 02/TODO 03의 코드를 비교해보세요.


![TODO03](https://raw.githubusercontent.com/lightsh/jsstudy/master/16-2015년01월14일/todo/images/todo_02.gif)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
		
		.panel {
			margin-bottom: 20px;
			background-color: #fff;
			border: 1px solid transparent;
			border-color: #ddd;
			border-radius: 4px;
			box-shadow: 0 1px 1px rgba(0,0,0,.05);
		}
		
		.panel-heading {
			padding: 10px 15px;
			border-bottom: 1px solid transparent;
			border-top-right-radius: 3px;
			border-top-left-radius: 3px;
			color: #333;
			background-color: #f5f5f5;
			border-color: #ddd;			
		}
		
		.panel-body {
			padding: 10px 15px;			
		}
			
		a:hover { 
			text-decoration:underline;
			cursor:pointer;
		}
						
		</style>
		<script type="text/javascript">
			
				
		</script>
	</head>
<body>
	<h1> The fundamentals </h1>
	<div>
		<div>
			<div>What is ChattingCat?</div>
			<div>ChattingCat connects people who want someone to check their written English with people who want to help. This way, writers can get instant review and corrections of their writing.</div>
		<div>
		<div>
			<div>What is the origin of ChattingCat?</div>
			<div>April, the co-founder of ChattingCat, grew up in Korea but worked as a marketer in the US. April wrote English for many things: emails to customers, text on the company website, etc.

	To write “like a native speaker”, April hired a tutor and texted him her writing. The tutor sent corrections back immediately. Instant corrections helped April work efficiently and fast.

	April was convinced that instant correction of her mistakes helped her learn quickly. With instant correction, she could write, see mistakes and learn. With instant help, she felt confident writing, and wanted to write more.

	That’s how ChattingCat was born!
			</div>
		</div>
		<div>
			<div>What is the vision for ChattingCat?</div>
			<div>The vision for ChattingCat: “Everyone should feel free to write in another language and connect with anyone.”</div>
		</div>
		<div>
			<div> For Students, how does ChattingCat work?</div>
			<div>On ChattingCat, people who want someone to check their writing are called Students.

	When a Student joins ChattingCat, they receive 5 catnip, ChattingCat’s virtual currency. When Students use catnip, they can upload English sentences for correction. 70 characters costs one catnip. 700 characters costs ten catnip.
			</div>
		</div>
		<div>
			<div>For Tutors, how does ChattingCat work?</div>
			<div>On ChattingCat, people who correct writing are called Tutors. To join ChattingCat as a Tutor, you need to pass a test. When you pass, you join as a Trainee and you can correct sentences for Students. After each correction, Students rate your corrections from one to five points.

	After you have received an average rating of 3.5/5.0 points or above for 20 corrections, ChattingCat will review your work and upgrade you to the Experienced tutor level.

	As an experienced tutor, you can collect catnip and trade it for cash.
			</div>	
		</div>
	</div>
</body>
</html>

```

TODO 01
========

* 아래 total_payment 함수를 구현해주세요.
* 전역 변수 사용하지 마세요.

```javascript

function total_payment(list) {

	//
	// TO DO 
	// 1. 인자 list 은 쇼핑 목록을 담은 배열입니다.
	// 2. 쇼핑 아이템의 구매 금액은 개수 x 단가(count * price) 입니다.
	// 3. 전체 구매 금액을 린턴해주세요.
	// 
}
		
		
```

> 초기 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/10/todo/images/todo_01.png)


>  결과 화면

![TODO01](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/10/todo/images/todo_01_result.png)

## HTML template

```html

<!DOCTYPE html> 
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
		
			function total_payment(list) {

			}
		
			
			window.onload = function() {
			
					document.getElementById("buy").onclick = function() {
					
					var shoppinglist = [];
					
					shoppinglist.push({"id" : "penny", "item" : "handbag", "count" : 1, "price" : 1000});
					shoppinglist.push({"id" : "penny", "item" : "skin", "count" : 2, "price" : 300});
					shoppinglist.push({"id" : "lenord", "item" : "iphone", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "lenord", "item" : "television", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "sheldon", "item" : "book", "count" : 10, "price" : 100});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					
										
					document.getElementById("payment").value = total_payment(shoppinglist);
				};
			}			
		</script>
	</head>
<body>               
	<input type="button" id="buy" value="buy"/>
    <br>	
    <textarea id="payment">
	</textarea>
</body>
</html>

```

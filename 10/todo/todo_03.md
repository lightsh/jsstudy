TODO 03
========

* 아래 total_payment_by_id,  print_payment 함수를 구현해주세요.
* 전역 변수 사용하지 마세요.


```javascript

function total_payment_by_id(soldoutlist, shoppinglist) {

	//
	// TO DO 
	// 1. 인자 shoppinglist 은 쇼핑 목록을 담은 배열입니다.
	// 2.(*) 인자 soldoutlist 은 품절된 상품 목록을 담은 배열입니다.
	// 3.(*) 금액을 계산할 때 품절된 상품은 제외시켜 주세요.
	// 4. 쇼핑 아이템의 구매 금액은 개수 x 단가(count * price) 입니다.
	// 5. 아이디별 전체 구매 금액을 배열(또는 객체, 마음대로 ~~, 단 문자열은 안됨)로 린턴해주세요.
	// 
}


function print_payment(list) {

	//
	// TO DO 
	// 1. 인자 list 은 아이디별 구매 금액을 담은 배열(또는 객체, 마음대로 ~~, 단 문자열은 안됨)입니다.
	// 2. 아래처럼 문자열을 리턴해주세요.
	//
	//    {아이디#1}: {구매금액#1}원 
    //    {아이디#2}: {구매금액#2}원 
    //    {아이디#3}: {구매금액#3}원 
    //    ------------------------ 
    //    Total : {구매금액총합}원 
	// 
}
			
		
		
```

> 초기 화면

![TODO03](https://raw.githubusercontent.com/lightsh/jsstudy/master/10/todo/images/todo_03.png)


>  결과 화면

![TODO03](https://raw.githubusercontent.com/lightsh/jsstudy/master/10/todo/images/todo_03_result.png)

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
		
			function total_payment_by_id(soldoutlist, shoppinglist) {

			}
			
		
			function print_payment(list) {
			
			}
			
			window.onload = function() {
			
					document.getElementById("buy").onclick = function() {
					
					var soldoutlist = [];
					
					soldoutlist.push("mouse");
					soldoutlist.push("handbag");
					
					var shoppinglist = [];
					
					shoppinglist.push({"id" : "penny", "item" : "handbag", "count" : 1, "price" : 1000});
					shoppinglist.push({"id" : "penny", "item" : "skin", "count" : 2, "price" : 300});
					shoppinglist.push({"id" : "lenord", "item" : "iphone", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "lenord", "item" : "television", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "sheldon", "item" : "book", "count" : 10, "price" : 100});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					
										
					document.getElementById("payment").value = print_payment(total_payment_by_id(soldoutlist, shoppinglist));
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

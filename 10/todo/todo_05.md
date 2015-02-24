TODO 05
========

* 아래 total_payment_by_id,  print_payment 함수를 구현해주세요.
* 전역 변수 사용하지 마세요.


```javascript

function total_payment_by_id(blacklist, stocklist, shoppinglist) {

	//
	// TO DO 
	// 1. 인자 shoppinglist 은 쇼핑 목록을 담은 배열입니다.
	// 2. 인자 stocklist 은 상품별 재고 목록을 담은 배열입니다.
	// 3.(*) 인자 blacklist 은 블랙 리스트를 담은 배열입니다.(블랙 리스트는 불량 고객에 대한 id 를 포함))
	// 4. 금액을 계산할 때 주문한 개수(count)보다 재고가 적으면 재고 개수(remains)로 금액을 계산해주세요.
	//
	//    if({주문개수} > {재고개수}) 
	//        재고개수 * 단가
	//    else
	//        주문개수 * 단가
	// 5. 재고 목록에 상품이 없는 경우에도 계산에서 빼주세요.
	// 6.(*)블랙 리스트에 포함되는 불량 고객은 구매가 불가합니다. 계산에서 빼주세요.
	// 7. 쇼핑 아이템의 구매 금액은 개수 x 단가(count * price) 입니다.
	// 8. 아이디별 전체 구매 금액을 배열(또는 객체, 마음대로 ~~, 단 문자열은 안됨)로 린턴해주세요.
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

![TODO05](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/10/todo/images/todo_05.png)


>  결과 화면

![TODO05](https://github.com/ByungChangYoo/clipsoft/blob/master/javascript/10/todo/images/todo_05_result.png)

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
		
			function total_payment_by_id(blacklist, stocklist, shoppinglist) {

			}
			
			function print_payment(list) {
			
			}
			
			window.onload = function() {
			
					document.getElementById("buy").onclick = function() {
					
					var stocklist = [];
					var blacklist = [];
					var shoppinglist = [];

					stocklist.push({"item" : "handbag", "remains" : 2});
					stocklist.push({"item" : "skin", "remains" : 1});
					stocklist.push({"item" : "iphone", "remains" : 2});
					stocklist.push({"item" : "television", "remains" : 0});
					stocklist.push({"item" : "book", "remains" : 5});
					stocklist.push({"item" : "mouse", "remains" : 1});

					blacklist.push("penny");
					blacklist.push("sheldon");
					blacklist.push("euhgene");
					blacklist.push("jessica");
										
					shoppinglist.push({"id" : "penny", "item" : "handbag", "count" : 1, "price" : 1000});
					shoppinglist.push({"id" : "penny", "item" : "skin", "count" : 2, "price" : 300});
					shoppinglist.push({"id" : "lenord", "item" : "iphone", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "lenord", "item" : "television", "count" : 1, "price" : 6000});
					shoppinglist.push({"id" : "sheldon", "item" : "book", "count" : 10, "price" : 100});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					shoppinglist.push({"id" : "sheldon", "item" : "mouse", "count" : 1, "price" : 5000});
					
										
					document.getElementById("payment").value = print_payment(total_payment_by_id(blacklist, stocklist, shoppinglist));
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

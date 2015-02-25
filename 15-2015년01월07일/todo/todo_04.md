TODO 04
========

* 아래 코드를 복사/붙여넣기 내공을 사용하십시오.
* CSS 에 아래 내용을 추가해주세요.
```css
		<style type="text/css">
			ul.miniTabHeader { margin:0 10px; padding:0; text-align:left; }
			ul.miniTabHeader li { list-style:none; display:inline; margin:0; padding:0; }
			ul.miniTabHeader li a { border:1px solid #E0E0E0; padding:3px 6px; background:#F0F0F0; font-size:14px; text-decoration:none; font-family:Georgia, "Times New Roman", Times, serif; }
			ul.miniTabHeader li a:hover { background-color:#F6F6F6; }
			ul.miniTabHeader li a.current { background:#fff; color:#222; border-bottom:1px solid #fff; }
			div.miniTabContent { border:1px solid #E0E0E0; padding:5px 15px 15px; margin-top:3px; display:none;}
		</style>
``` 

* HTML은 수정하지 말고 JavaScript 만을 사용해서 구현해주세요.

> 초기 화면
![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/15-2015년01월07일/todo/images/todo_04_01.png)


> Tutorial : Writing a game program in JavaScript – Introduction 클릭했을 때 화면
![TODO04](https://raw.githubusercontent.com/lightsh/jsstudy/master/15-2015년01월07일/todo/images/todo_04_02.png)

## HTML template

```html

<!DOCTYPE html> 
<html>
	<head>
		<meta charset="UTF-8">
		<style type="text/css">
			ul.miniTabHeader { margin:0 10px; padding:0; text-align:left; }
			ul.miniTabHeader li { list-style:none; display:inline; margin:0; padding:0; }
			ul.miniTabHeader li a { border:1px solid #E0E0E0; padding:3px 6px; background:#F0F0F0; font-size:14px; text-decoration:none; font-family:Georgia, "Times New Roman", Times, serif; }
			ul.miniTabHeader li a:hover { background-color:#F6F6F6; }
			ul.miniTabHeader li a.current { background:#fff; color:#222; border-bottom:1px solid #fff; }
			div.miniTabContent { border:1px solid #E0E0E0; padding:5px 15px 15px; margin-top:3px; display:none;}
		</style>
		<script type="text/javascript">
			
		</script>
	</head>
<body>
    <h1> Tutorial : Writing a game program in JavaScript </h1>
    <div class="miniTab">
		<ul class="miniTabHeader">
		    <li ><a href="#">Tutorial : Writing a game program in JavaScript – Introduction</a></li>
		    <li><a href="#">Tutorial : Writing a game program in JavaScript – Part 1</a></li>
		    <li><a href="#">Tutorial : Writing a game program in JavaScript – Part 2</a></li>
		</ul>
		<div class="miniTabContent">    
			In this tutorial, I’m going to explain how to write a game program in JavaScript. Before starting off this tutorial, let me get something straight. I’m also a newbie JavaScript learner, and I’ve never make any other games before. To be honest, it’s my first tutorial and I’ve been shying away from posting this tutorial because I’m worried about telling something every JavaScript developers already know very well in a different way.

Eventually, I decided to post this tutorial. I thought that it would be worth posting my humble tutorial for every JavaScript learner in the world, even if it’s about a simple and terrible game. Conversely, it could be a suitable tutorial for beginners, because it’s about a super simple and humble game. It means that this tutorial might be easy to understand. As a result, it could give you confidence in your ability enough to make more awesome games than the game I made in this tutorial.

First of all, you should know that the game we’re going to make is based on an HTML table and CSS. I will try to do my best to make this tutorial understandable and keep it as simple as possible. However, there is one thing I expect of you :  I expect you to already have a basic understanding of WEB programming in order to be able to follow this tutorial, because I don’t have any plan to explain what HTML is, what CSS is, what JavaScript is, and so on. If you are an experienced JavaScript developer, this might be not so much the tutorial you’re looking for as the one you’re really trying to avoid. I don’t mind if you press the back button on your browser without leaving your comment about this tutorial.

You don’t need to start from scratch. I will provide you with an HTML page for helping you focus on just writing a code. You can start with the following code snippet that I made.
		</div>

		<div class="miniTabContent">  
		The game consists of two parts: a player and enemies. A player can be controlled with the arrow keys, whereas enemies cannot be. Enemies are just targets that the player should kill.

Let’s first focus on adding a player to the game. We’re going to make one of the cells in the table the player, whose background color is blue, and then give him the ability to move from right to left. You can make the player move in the direction you want by pressing the left (←) or right (→) arrow key. If you press the up (↑) or down (↓)arrow key, the player has no idea what you are asking for. Note that the player cannot move up and down in the game.
		</div>
		<div class="miniTabContent">
In the previous post, we gave the player the ability to move where the user wanted. Imagine that the player has just one ability to move from left to right in the game: there is no doubt that users would get bored and lose their interest in playing the game. I recently stumbled across a funny and bitter article. According to the article, most of the people who are the third wheel think of their coupled-off friends as a constant reminder of their bitter loneliness. The article encourages me to add a special ability to the game to stop it from being the third wheel. We’re just taking baby steps at the moment, but I’m convinced that we will make a little progress on the game in this post.

It is time to give a special ability to the player: it makes the game more dynamic and gets your attention. That is the firepower, which means the player can fire bullets. When the user press the spacebar (” “) key, the player would fire the bullet which is supposed to go toward the top of the table.</div>
	</div>
</body>
</html>

```

<script>
	export let name;
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Mono:wght@400;500&display=swap');
:global(body) {
	background-color:  #282c34;
	text-align: center;
	align-items: center;
}
.ada-title {
	font-family: 'Fira Mono', monospace;
	color: white;
	font-size: 55px;
	transition: 0.25s;
}
.ada-title:hover {
	letter-spacing: 1.2px;
	font-size: 56px;
}
:global(input) {
	border-radius: 5px;
	font-family: 'Fira Mono', monospace;
	font-weight: 400;
	transition: 0.2s;
	width: 210px;
}
:global(input):hover {
	background-color:darkgray;
}
:global(button) {
	border-radius: 7px;
	color: white;
	border: 0;
	width: 210px;
	background-color:#376fc9;
	transition: 0.2s;
}
:global(button):hover {
	background-color:#4183ec;
}
:global(button):focus {
	color: black;
}
</style>
<main>
	<br><br><br><br><br><br><br><br>
	<h1 class="ada-title">News</h1><br>
	<form method="post">
	<input type="text" placeholder="Username" name="uname" required>
	<br>
	<input type="password" placeholder="Password" name="psw" required>
	<br><br>
	<button type="submit">Log In</button>
	<br>
	<button type="submit">Sign Up</button>
</form>
</main>


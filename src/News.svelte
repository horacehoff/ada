<script>
	import Post from './Post.svelte'
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Fira+Mono:wght@400;500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Shippori+Antique+B1&display=swap');
:global(body) {
	background-color:  #282c34;
	text-align: center;
	align-items: center;
}
.ada-title {
	font-family: 'Fira Mono', monospace;
	color: white;
	font-size: 40px;
}
</style>
<main>
	<br><br>
	<h1 class="ada-title">Ada News</h1><br>
	<Post title="AWESOME" description="It works!" img_url="https://i.ytimg.com/vi/7DVOaPqwgMU/maxresdefault.jpg"/>
</main>


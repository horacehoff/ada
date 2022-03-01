<script>
    export let title;
    export let img_url;
    export let description;
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Shippori+Antique+B1&display=swap');
.post {
    display: inline-block;
    width: 455px;
    height: 296px;
    background-color: rgb(59, 56, 56);
    border-radius: 10px;
    overflow: hidden;
    transition: 0.3s;
    margin: 15px;
}
.post:hover {
	box-shadow: 0px 0px 1px rgba(0, 0, 0, 0.9), 0px 4px 20px rgba(0, 0, 0, 0.25);
}
.post-title {
	color: rgb(255, 255, 255);
	white-space: nowrap;
	font-size: 18px;
	font-family: 'Shippori Antique B1', sans-serif;
}
.post-image {
	background: url("https://www.levert.ma/wp-content/uploads/2020/11/greenpeace-678x381.jpg") no-repeat center center;
  	background-size: cover;
	height: 100px;
	width: 455px;
}
.post-description {
	color: white;
	font-family: 'Shippori Antique B1', sans-serif;
}
.justify-text {
	text-align: justify;
	padding-right: 20px;
	padding-left: 20px;
}
</style>
<div class="post">
    <div id="background" class="post-image" style="background: url('{img_url}') no-repeat center center"></div>
    <h3 class="post-title">{title}</h3>
    <div class="justify-text">
    <p class="post-description">{description}</p>
    </div>
</div>
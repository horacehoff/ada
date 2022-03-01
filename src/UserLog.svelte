<script>
import { user } from './user';
  let username;
  let password;
  function login() {
    user.auth(username, password, ({ err }) => err && alert(err));
  }
  function signup() {
    user.create(username, password, ({ err }) => {
      if (err) {
        alert(err);
      } else {
        login();
      }
    });
  }
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
	color: white;
	border: 0;
	width: 210px;
	background: linear-gradient(180deg, #3B7ADD 0%, #346DC5 100%);
	/* Alert/Button/Default glow [D] */
	box-shadow: 0px 0.5px 1.5px rgba(0, 0, 0, 0.25), inset 0px 0.8px 0px -0.25px rgba(255, 255, 255, 0.2);
	border-radius: 6px;
}
:global(button):focus {
	background-color:#346DC5;
	color: white;
}
</style>
<main>
	<br><br><br><br><br><br><br><br>
	<h1 class="ada-title">Ada</h1><br>
	<input type="text" placeholder="Username" name="uname" bind:value={username} minlength="5" maxlength="16" required>
	<br>
	<input type="password" placeholder="Password" name="psw" bind:value={password} required>
	<br><br>
	<button on:click={login}>Log In</button>
	<br>
	<button on:click={signup}>Sign Up</button>
</main>


<script context="module">
	import { SvelteComponent } from 'svelte'
	import News from './News.svelte'
	import UserLog from './UserLog.svelte'
	let Views = [UserLog, News]
	let MainComponent = Views[0]
	export function change() {
		console.log('Debug')
		MainComponent = Views[1]
	}	
</script>
<div id="main">
	<svelte:component this={MainComponent} id="svelteComp"/>
</div>


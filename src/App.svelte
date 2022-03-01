<script context="module">
	import UserLog from './UserLog.svelte'
	import News from './News.svelte'
	const views = [UserLog, News]

	let viewportComponent = null
	let currentView = 0
	
	export function toggleView() {
		currentView = currentView == 0 ? 1 : 0
	}

	export function updateViewportComponent() {
		viewportComponent = views[currentView]
	}
	updateViewportComponent()
</script>
<div id="main">
	<svelte:component this={viewportComponent}/>
</div>


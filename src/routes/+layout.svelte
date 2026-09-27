<script>
	import { page } from '$app/state';
	let { children } = $props();
</script>

<nav><a id="home" href="/">home</a> <a id="fail" href="/fail">fail</a> <a id="ok" href="/ok">ok</a></nav>

{#if page.error}
	{@render children()}
{:else}
	<main>{@render children()}</main>
{/if}

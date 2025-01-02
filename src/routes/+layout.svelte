<script>
	import '../app.css';
	import { base } from "$app/paths";
	import Header from '$lib/components/Header.svelte'
	
	let { children } = $props();
</script>

<Header />
<div class="font-bold bg-sky-50">
<a href="{base}/">Home</a> &nbsp; &nbsp;
<a href="{base}/cv">CV</a> &nbsp; &nbsp;
<a href="{base}/photos">Photos</a> &nbsp; &nbsp;
<a href="{base}/privacy">Privacy</a>
</div>

{@render children()}

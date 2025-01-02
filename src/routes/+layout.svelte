<script>
	import '../app.css';
	import { base } from "$app/paths";
	
	let { children } = $props();

  //import '$lib/styles/style.css'
  //import Header from '$lib/components/Header.svelte'
</script>


<div class="font-bold bg-blue-100">
<a href="{base}/">Home</a> &nbsp; &nbsp;
<a href="{base}/cv">CV</a> &nbsp; &nbsp;
<a href="{base}/photos">Photos</a> &nbsp; &nbsp;
<a href="{base}/privacy">Privacy</a>
<br />
</div>

{@render children()}

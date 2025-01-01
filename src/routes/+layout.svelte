<script>
	import '../app.css';
	import { base } from "$app/paths";
	
	let { children } = $props();


  //import { base } from "$app/paths";
  //import '$lib/styles/style.css'
  //import Header from '$lib/components/Header.svelte'
  //import "../app.css";
</script>


<div class="nav" style="background-color: AliceBlue;">
<a href="{base}/">Home</a> &nbsp; &nbsp;
<a href="{base}/cv">CV</a> &nbsp; &nbsp;
<a href="{base}/privacy">Privacy</a>
<br />
</div>



{@render children()}

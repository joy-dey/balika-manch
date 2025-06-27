<script>
	import '../app.css';
	import { Navbar, Footer } from '$lib';
	import { injectSpeedInsights } from '@vercel/speed-insights/sveltekit';

	injectSpeedInsights();

	let { children } = $props();
</script>

<Navbar></Navbar>
{@render children()}
<Footer></Footer>

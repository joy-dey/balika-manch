<script>
	import '../app.css';
	import { Navbar, Footer } from '$lib';

	let { children } = $props();
</script>

<Navbar></Navbar>
{@render children()}
<Footer></Footer>

<script>
	import '../app.css';
	import Footer from '../lib/Footer.svelte';
	import Header from '../lib/Header.svelte';
</script>

<div class="bg-black mx-auto max-w-screen-md my-4 rounded-xl p-8">
	<Header />
	<slot />
	<Footer />
</div>

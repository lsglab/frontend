<script>
	/* eslint-disable sort-imports-es6-autofix/sort-imports-es6 */
	import Tailwind from '../components/atoms/Tailwind.svelte';
	import Styles from '../components/atoms/Styles.svelte';
	import Footer from '../components/organisms/Footer.svelte';
	import Nav from '../components/organisms/Nav.svelte';
</script>

<svelte:head>
	<title>{process.globals.title}</title>
</svelte:head>

<Tailwind />
<Styles />
<Nav />
<slot />
<Footer />

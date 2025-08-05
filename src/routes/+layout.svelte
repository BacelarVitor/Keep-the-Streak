<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
    import '../global.css'
    import '@picocss/pico/css/pico.css';

	let { children } = $props();
</script>

<style>
    main {
        padding-top: 3rem;
    }
</style>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>
  
<main class="container">
	{@render children?.()}
</main>


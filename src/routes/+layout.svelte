<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

<main class="flex flex-col gap-4 p-8 h-full items-center justify-center">
	{@render children()}
</main>

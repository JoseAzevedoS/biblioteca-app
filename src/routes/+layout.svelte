<script lang="ts">
	import Cabecalho from "$lib/componentes/Cabecalho.svelte";
	let { children } = $props();
	import '../app.css'
</script>

<Cabecalho></Cabecalho>
{@render children()}
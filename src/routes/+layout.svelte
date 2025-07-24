<script lang="ts">
	import Cabecalho from "$lib/componentes/Cabecalho.svelte";
	import Rodape from "$lib/componentes/Rodape.svelte";
	let { children } = $props();
	import '../app.css'
</script>

<Cabecalho></Cabecalho>

{@render children()}
<Rodape></Rodape>
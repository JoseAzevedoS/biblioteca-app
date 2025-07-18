<script lang="ts">
	import Cabecalho from "$lib/componentes/Cabecalho.svelte";
	import Rodape from "$lib/componentes/Rodape.svelte";
	import Menu from "$lib/componentes/menu.svelte";
	let { children } = $props();
	import '../app.css'
</script>

<Cabecalho></Cabecalho>
<Menu></Menu>
<Rodape></Rodape>
{@render children()}
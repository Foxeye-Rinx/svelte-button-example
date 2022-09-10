<script>
	import Button from '$lib/Button.svelte';
	function handleClick() {
		console.log('clicked');
	}
</script>

<Button on:click={handleClick}>My Button</Button>
<Button on:click={handleClick} colorProfile="red">Red Button</Button>

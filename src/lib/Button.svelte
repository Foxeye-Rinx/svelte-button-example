<script>
	export let colorProfile = '';
</script>

<button class="btn" class:red={colorProfile === 'red'} on:click>
	<slot />
</button>

<style>
	.btn.red {
		color: rgb(255, 42, 42);
		background: rgb(255, 228, 231);
		border-color: rgb(255, 142, 153);
	}
	.btn.red:hover {
		background: rgb(255, 192, 192);
		border-color: rgb(255, 130, 142);
	}
	.btn {
		border: 1px solid rgb(209, 213, 219);
		border-radius: 0.375rem;
		cursor: pointer;
		padding: 0.375rem 1rem;
		font-size: 100%;
		background-color: inherit;
		color: #212121;
	}
	.btn:hover {
		border-width: 1px;
		border-radius: 0.375rem;
		border-color: rgb(164, 164, 164);
		background-color: rgb(238 238 238);
	}
</style>

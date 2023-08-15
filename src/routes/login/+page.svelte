<script>
	async function handleSubmit() {
		const response = await fetch('');
		const data = await response.json();
	}
</script>

<div class="flex flex-col gap-2">
	<label class="label">
		<span>Username</span>
		<input class="input" type="text" placeholder="username..." />
	</label>
	<label class="label">
		<span>Password</span>
		<input class="input" type="password" placeholder="*****" />
	</label>
	<button class="btn variant-filled-secondary mt-2" on:click={handleSubmit}>Submit</button>
</div>

<script>
	import '../app.css';
    import Input from '$lib/Input.svelte';
</script>

<fieldset class="fieldset bg-base-200 border-base-300 rounded-box w-xs border p-4">
	<div class="grid grid-cols-2 gap-x-8 gap-y-4 text-left">
		<div>
			<label class="label">Email</label>
			<input type="email" class="input" placeholder="Email" />

			<label class="label">Password</label>
			<input type="password" class="input" placeholder="Password" />

			<button class="btn btn-neutral mt-4">Login</button>
		</div>

		<div>
			<label class="label">Email</label>
			<input type="email" class="input" placeholder="Email" />

			<label class="label">Password</label>
			<input type="password" class="input" placeholder="Password" />

			<button class="btn btn-neutral mt-4">Login</button>
            <Input />
		</div>
	</div>
</fieldset>

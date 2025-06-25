<script lang="ts">
	let {
		id = '',
		placeholder = '',
		required = false,
		pattern = '^\\d{9}$',
		value = $bindable() as string
	} = $props();

	let isValid = $state(true);

	// Debug tools
	$inspect(isValid).with(console.trace);
	$inspect(value).with(console.trace);

	// Validation
	function validate() {
		if (required && value.trim() === '') {
			isValid = false;
		} else if (pattern) {
			const regex = new RegExp(pattern);
			isValid = regex.test(value);
		} else {
			isValid = true;
		}
	}
</script>

<div>
	<input
		class="input focus:outline-none"
		{id}
		{placeholder}
		{required}
		onblur={validate}
		oninput={validate}
		bind:value
	/>
</div>

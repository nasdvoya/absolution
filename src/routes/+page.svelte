<script>
	import '../app.css';
	import Input from '$lib/Input.svelte';
</script>

<fieldset class="fieldset bg-base-200 border-base-300 rounded-box w-xs border p-4">
	<div class="grid grid-cols-2 gap-x-8 gap-y-4 text-left">
		<div>
			<label class="label" for="name">Nome</label>
			<Input id="name" />

			<label class="label" for="email">Email</label>
			<Input id="email" />

			<label class="label" for="horario">Horário</label>
			<Input id="horario" />

			<label class="label" for="doador">Doador</label>
			<Input id="doador" />
		</div>

		<div>
			<label class="label" for="freguesia">Freguesia</label>
			<Input id="freguesia" />

			<label class="label" for="concelho">Concelho</label>
			<Input id="concelho" />

			<label class="label" for="codigopostal">Código postal</label>
			<Input id="codigopostal" />

			<label class="label" for="telresidencial">Tel. Residencial</label>
			<Input id="telresidencial" />

			<label class="label" for="teltrabalho">Tel. Trabalho</label>
			<Input id="teltrabalho" />

			<label class="label" for="telemovel">Telemóvel</label>
			<Input id="telemovel" />
		</div>
	</div>
</fieldset>

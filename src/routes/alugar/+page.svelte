<script lang="ts">
	import { enhance } from '$app/forms';
	let loading = $state(false);
</script>

<header>
	<nav class="navbar px-6" aria-label="main navigation">
		<div class="navbar-brand">
			<a class="navbar-item has-text-weight-semibold" href="https://bulma.io">
				<span style="color: #EF7D00">HomeShop</span>
			</a>
			<a
				role="button"
				class="navbar-burger"
				aria-label="menu"
				aria-expanded="false"
				data-target="navbarBasicExample"
			>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
				<span aria-hidden="true"></span>
			</a>
		</div>

		<div id="navbarBasicExample" class="navbar-menu">
			<div class="navbar-start">
				<a href="/alugar" class="navbar-item has-text-weight-semibold">Alugar</a>
				<a href="/comprar" class="navbar-item has-text-weight-semibold">Comprar</a>
				<a href="/vender" class="navbar-item has-text-weight-semibold">Vender</a>
			</div>

			<div class="navbar-end">
				<div class="navbar-item pr-0">
					<div class="buttons">
						<a class="button is-primary has-text-warning">
							<strong>Sign up</strong>
						</a>
						<a class="button is-light">Log in</a>
					</div>
				</div>
			</div>
		</div>
	</nav>
</header>

<div class="section">
	<form
		class="card is-primary"
		method="POST"
		use:enhance={() => {
			loading = true;
			return async ({ update }) => {
				await update();
				loading = false;
			};
		}}
	>
		<div class="card-content">
			<div class="field">
				<label class="label" for="name">Cidade</label>
				<div class="control has-icons-left">
					<input
						id="cidade"
						class="input"
						name="cidade"
						type="text"
						placeholder="Digite o nome da cidade"
					/>
					<span class="icon is-left">
						<i class="fa-regular fa-house fa-fw"></i>
					</span>
				</div>
			</div>
			<div class="field">
				<label class="label" for="name">Bairro</label>
				<div class="control has-icons-left">
					<input
						id="bairro"
						class="input"
						name="bairro"
						type="text"
						placeholder="Digite o nome do bairro"
					/>
					<span class="icon is-left">
						<i class="fa-solid fa-location-dot fa-fw"></i>
					</span>
				</div>
			</div>
			<div class="field-body">
				<div class="field">
					<label class="label" for="name">Valor mínimo</label>
					<div class="control has-icons-left">
						<input
							id="minimo"
							class="input"
							name="minimo"
							type="number"
							placeholder="Valor mínimo"
						/>
						<span class="icon is-left">
							<i class="fa-solid fa-dollar-sign fa-fw"></i>
						</span>
					</div>
				</div>
				<div class="field">
					<label class="label" for="name">Valor máximo</label>
					<div class="control has-icons-left">
						<input
							id="maximo"
							class="input"
							name="maximo"
							type="number"
							placeholder="Valor máximo"
						/>
						<span class="icon is-left">
							<i class="fa-solid fa-dollar-sign fa-fw"></i>
						</span>
					</div>
				</div>
			</div>
			<div class="columns mt-2">
				<div class="column is-full-mobile is-2-tablet" style="min-width: 200px">
					<button
						aria-busy={loading}
						class:is-loading={loading}
						class="button is-primary is-fullwidth has-text-white has-text-weight-semibold"
						type="submit"
					>
						<i class="fa-solid fa-magnifying-glass fa-fw">&nbsp;</i>Pesquisar
					</button>
				</div>
			</div>
		</div>
	</form>
	<div class="columns is-flex-wrap-wrap">
		{#each { length: 8 }, rank}
			<div class="column is-3">
				<div class="card">
					<div class="card-image">
						<a href="/alugar/623e4925-c9a6-4d48-8377-659868b03538">
							<img
								class="image is-120x120"
								src="https://placehold.co/680x240/EEE/31343C"
								alt="Placeholder"
							/>
						</a>
					</div>
					<div class="card-content">
						<div class="media">
							<div class="media-left">
								<figure class="image is-48x48">
									<img
										src="https://bulma.io/assets/images/placeholders/96x96.png"
										alt="Placeholder"
									/>
								</figure>
							</div>
							<div class="media-content">
								<p class="title is-4">Apartamento</p>
								<p class="subtitle is-6">@johnsmith</p>
							</div>
						</div>

						<div class="content">
							Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.<a
								href="#">#css</a
							>
							<a href="#">#responsive</a>
							<br />
							<time datetime="2016-1-1">11:09 PM - 1 Jan 2016</time>
						</div>
					</div>
				</div>
			</div>
		{/each}
	</div>
</div>

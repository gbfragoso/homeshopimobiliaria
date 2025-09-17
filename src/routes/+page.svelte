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
				<div class="navbar-item">
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

<section id="hero" class="hero is-fullheight">
	<div class="hero-body">
		<div class="card">
			<div class="card-content">
				<form action="" method="POST">
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
					<div class="field">
						<div class="control">
							<button class="mt-3 button is-primary has-text-warning has-text-weight-semibold"
								>Buscar</button
							>
						</div>
					</div>
				</form>
			</div>
		</div>
	</div>
</section>

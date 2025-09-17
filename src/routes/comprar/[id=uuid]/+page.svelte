<script lang="ts">
	let options = { loop: false };
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

<section class="section">
	<div class="content">
		<h3>Apartamento, Salvador, Bahia</h3>

		<h4>Sobre o local</h4>
		<p>
			A 1,5km do Centro de Convenções de Salvador. A 800 metros do local de shows da Virada, na
			Arena Canto da cidade.
		</p>
		<p>
			Temos um pequeno shopping com várias lojas e restaurantes ao redor 2. Praia corsário a 200
			metros, com bike Itaú e patinetes na Nova orla
		</p>
		<ul>
			<li>In fermentum leo eu lectus mollis, quis dictum mi aliquet.</li>
			<li>Morbi eu nulla lobortis, lobortis est in, fringilla felis.</li>
			<li>Aliquam nec felis in sapien venenatis viverra fermentum nec lectus.</li>
			<li>Ut non enim metus.</li>
		</ul>
	</div>
</section>

<section class="section">
	<div class="content">
		<h4>O que esse lugar oferece</h4>
		<p>
			<i class="fa-solid fa-shower"></i> 2 Banheiros
		</p>
		<p>
			<i class="fa-solid fa-car"></i> 1 Garagem
		</p>
		<p>
			<i class="fa-solid fa-bed"></i> 3 Quartos
		</p>
	</div>
</section>

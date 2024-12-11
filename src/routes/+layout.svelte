<script>
	import Logo from '$lib/assets/true_steadywinsLogoDark.svg'
</script>

<nav>
	<div class="logo">
		<!-- svelte-ignore a11y_missing_attribute -->
		<img src={Logo} class="logo__image" />
		<div class="logo__text">Steady Wins Design</div>
	</div>
	<ul>
		<li><a href="/">Home</a></li>
		<li><a href="/about">About</a></li>
		<li><a href="/myWork">My Work</a></li>
	</ul>
</nav>
<slot />

<style>
	nav {
		display: flex;
		justify-content: space-between;
		padding: 1rem 4rem;
    align-items: flex-end;
	}

	.logo {
		display: flex;
		align-items: end;
	}

	.logo__image {
		width: 112px;
		margin-right: 1rem;
	}

	.logo__text {
		font-size: 2.25rem;
		font-weight: 500;
	}

	ul {
		display: flex;
		list-style: none;
    margin-bottom: 0.25rem;
	}

	li {
		font-size: 1.25rem;
		font-weight: 500;
		margin-left: 1.75rem;
    transition: all 0.3s linear;
	}

  li:hover {
    transform: scale(1.1);
  }

	a {
		text-decoration: none;
	}
</style>

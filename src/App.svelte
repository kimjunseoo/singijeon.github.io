<script>
  import Header from "./lib/components/Header.svelte";
  import Footer from "./lib/components/Footer.svelte";
</script>

<Header />
<main>
	<div class="content">
		<h1>Singijeon</h1>
		<p>Easy, Simple and Fast Load Testing Tool</p>
		<p>Test stress quickly and secure stability through various response results</p>
		<div class="buttons">
			<a href="https://www.npmjs.com/package/singijeon" target="_blank">Get Started</a>
			<!-- <a href="https://www.npmjs.com/package/singijeon" target="_blank" class="secondary"
				>Learn more</a
			> -->
		</div>
	</div>
	<div class="image-placeholder">
		<img src="singijeon_demo.gif" alt="asdasd" />
	</div>
</main>

<section class="features">
	<div class="feature">
		<h3>Easy</h3>
		<p>You can test with a simple line of command through Cli</p>
	</div>
	<div class="feature">
		<h3>Simple</h3>
		<p>The barriers to entry are low. There is no study you need to do to use this tool</p>
	</div>
	<div class="feature">
		<h3>Fast</h3>
		<p>You can test often, many and quickly with this. More tests will be the better performance</p>
	</div>
</section>
<Footer />


<style>
	main {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 60px;
		flex-wrap: wrap;
	}

	.content {
		max-width: 600px;
		flex: 1 1 400px;
	}

	.content h1 {
		font-size: 2.5rem;
		margin-bottom: 10px;
	}

	.content p {
		font-size: 1rem;
		color: #555;
	}

	.buttons {
		margin-top: 30px;
	}

	.buttons a {
		text-decoration: none;
		padding: 10px 20px;
		background-color: #f98f00;
		color: #fff;
		border-radius: 5px;
		margin-right: 10px;
	}

	.buttons a.secondary {
		background-color: transparent;
		color: #000;
	}

	.image-placeholder {
		width: 100%;
		max-width: 400px;
		height: 300px;
		background-color: #000;
		flex: 1 1 400px;
		margin-top: 20px;
	}

	.features {
		display: flex;
		justify-content: space-around;
		margin-top: 40px;
		background-color: #fff;
		padding: 20px;
		border-radius: 10px;
		box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
		flex-wrap: wrap;
	}

	.feature {
		text-align: center;
		padding: 20px;
		flex: 1 1 200px;
	}

	.feature h3 {
		font-size: 1.25rem;
		margin-bottom: 10px;
	}

	.feature p {
		font-size: 0.9rem;
		color: #777;
	}

	@media (max-width: 768px) {
		main {
			flex-direction: column;
			align-items: flex-start;
		}

		.content h1 {
			font-size: 2rem;
		}

		.content p {
			font-size: 0.9rem;
		}

		.buttons a {
			padding: 8px 16px;
			margin-right: 5px;
		}

		.image-placeholder {
			height: 200px;
		}

		.features {
			flex-direction: column;
		}

		.feature {
			padding: 10px 0;
		}
	}

	@media (max-width: 480px) {
		.content h1 {
			font-size: 1.5rem;
		}

		.buttons a {
			display: block;
			margin: 10px 0;
		}

		.image-placeholder {
			height: 150px;
		}
	}
</style>

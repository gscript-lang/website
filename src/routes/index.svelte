<script lang="ts">
	function redirect(link: string) {
		window.open(link, "_blank")
	}
</script>

<div class="container">
	<h1>gScript©️</h1>
	<div class="links">
		<button on:click={() => redirect("https://www.npmjs.com/package/gscript-compiler")}>Compiler</button>
		<button on:click={() => redirect("https://github.com/gscript-lang/gscript")}>GitHub</button>
	</div>
</div>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@400;700&display=swap');

	.container {
		height: 100vh;
		width: 100vw;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: center;
		flex-direction: column;
		gap: 25px;
		font-family: 'Josefin Sans', sans-serif;

		h1 {
			color: white;
			font-weight: 700;
			font-size: 86px;
		}

		.links {
			display: flex;
			align-items: center;
			justify-content: space-between;
			max-width: 450px;
			flex-direction: row;
			gap: 25px;
			font-family: 'Josefin Sans', sans-serif; 

			button {
				background: #000;
				color: white;
				border: 2px solid white;
				border-radius: 8px;
				font-family: 'Josefin Sans', sans-serif;
				width: 150px;
				height: 60px;
				font-size: 24px;
				transition: 600ms ease-in-out;
				cursor: pointer;

				&:hover {
					background: #fff;
					color: black;
				}
			}
		}
	}
</style>
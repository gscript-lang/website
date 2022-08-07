<script lang="ts">
	function redirect(link: string) {
		window.open(link, "_blank")
	}
</script>

<div class="container">
	<div class="top">
		<h1>gScript©️</h1>
		<div class="links">
			<button on:click={() => redirect("https://www.npmjs.com/package/gscript-compiler")}>Compiler</button>
			<button on:click={() => redirect("https://www.npmjs.com/package/gscript-cli")}>CLI</button>
			<button on:click={() => redirect("https://github.com/gscript-lang/")}>GitHub</button>
		</div>
	</div>
	<h3>Made with ❤ by <a class="fx" href="https://molai.dev/">molai.dev</a> →</h3>
</div>

<style lang="scss">
	@import url('https://fonts.googleapis.com/css2?family=Josefin+Sans:wght@400;700&display=swap');

	.container {
		height: 100vh;
		width: 100vw;
		display: flex;
		align-items: center;
		justify-content: space-between;
		flex-direction: column;
		gap: 25px;
		font-family: 'Josefin Sans', sans-serif;

		.top {
			display: flex;
			margin-top: 350px;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			gap: inherit;

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

		h3 {
			color: white;
			font-size: 24px;
			margin-bottom: 25px;

			a {
				color: rgb(130, 130, 130);
				text-decoration: none;
			}
		}

		.fx {
        	    border: none;
        	    display: inline;
        	    position: relative;
        	    cursor: pointer;
        	    &:after {
        	        content: '';
        	        position: absolute;
        	        width: 100%;
        	        transform: scaleX(0);
        	        height: 2px;
        	        bottom: 0;
        	        left: 0;
        	        background-color: #0087ca;
        	        transform-origin: bottom right;
        	        transition: transform 0.25s ease-out;
        	    }	
        	    &:hover:after{
        	        transform: scaleX(1);
        	        transform-origin: bottom left;
        	    }
        	}
	}
</style>
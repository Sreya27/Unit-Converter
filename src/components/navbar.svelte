<script>
	let isMenuOpen = false;

	function toggleMenu() {
		isMenuOpen = !isMenuOpen;
	}

	let current = 0;
</script>

<div class="navbar">
	<a href="/" class="logo"><img id="logo-img" alt="logo symbol" src="https://drive.google.com/uc?export=view&id=1mrd6vE72fmDKJeVXrrVbOzxcXz93TSmJ"/></a>
	<nav class:open={isMenuOpen}>
		<ul>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)}>
				<a class:current={current === 0} on:click={() => (current = 0)} href="/">Length</a>
			</li>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)}>
				<a class:current={current === 1} on:click={() => (current = 1)} href="/">Temperature</a>
			</li>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)}>
				<a class:current={current === 2} on:click={() => (current = 2)} href="/">Volume</a>
			</li>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)}>
				<a class:current={current === 3} on:click={() => (current = 3)} href="/">Weight</a>
			</li>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)}>
				<a class:current={current === 4} on:click={() => (current = 4)} href="/">Time</a>
			</li>
			<!-- svelte-ignore a11y-click-events-have-key-events -->
			<li on:click={() => (isMenuOpen = false)} class="dropdown"><a on:click={() => (current = 5)} href="/">All Converters<svg fill="none" viewBox="0 0 24 24" height="24" width="24" xmlns="http://www.w3.org/2000/svg">
				<path xmlns="http://www.w3.org/2000/svg" d="M17 10L12 16L7 10H17Z" fill="#0D0D0D"></path>
				</svg></a></li>
		</ul>
	</nav>
	<button class="burger" on:click={toggleMenu}>
		<svg id="menu-bar" fill="none" viewBox="0 0 24 24" height="24" width="24" xmlns="http://www.w3.org/2000/svg">
			<path xmlns="http://www.w3.org/2000/svg" d="M4 7C4 6.44772 4.44772 6 5 6H19C19.5523 6 20 6.44772 20 7C20 7.55228 19.5523 8 19 8H5C4.44772 8 4 7.55228 4 7ZM4 12C4 11.4477 4.44772 11 5 11H19C19.5523 11 20 11.4477 20 12C20 12.5523 19.5523 13 19 13H5C4.44772 13 4 12.5523 4 12ZM4 17C4 16.4477 4.44772 16 5 16H19C19.5523 16 20 16.4477 20 17C20 17.5523 19.5523 18 19 18H5C4.44772 18 4 17.5523 4 17Z" fill="#0D0D0D"></path>
			</svg>
	</button>
</div>

<style>
	.navbar {
		background-color: white;
		display: flex;
		justify-content: space-between;
		align-items: center;
		position: relative;
        height: 4rem;
	}

	
	.logo img{
		width: 180px;
	}
	svg{

		position: relative;
		top: 5px;
	}

	
    @media only screen and (max-width: 767px){

    
        nav {
            display: none;
        }
        nav.open {
            display: block;
            position: absolute;
            top: 100%;
            left: 0;
            background-color: var(--light);
            width: 100%;
        }
    }

	ul {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		align-items: center;
		gap: 5vh;
		margin-top: 2vh;
		margin-bottom: 4vh;
		list-style: none;
		font-size: 1rem;
		font-weight: 600;
	}

	a{
		padding: 10px;
	}

	a:hover{
		background-color: white;
		border-radius: 10px;
	}
	.current {
		position: relative;
	}

	.current::after {
		content: '';
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 2px;
		background-color: var(--secondary);
	}

	.dropdown {
		background-color: var(--light);
		padding: 0.4rem 1rem;
		border-radius: 10px;
		font-weight: 600;
	}

	.burger{
		border: 0px;
		background-color: white;
		margin-bottom: 5px;
		margin-right: 10px;
	}
	
	.burger:hover{
		border: 0px;
		background-color: white;
		margin-bottom: 5px;
		margin-right: 10px;
		cursor: pointer;
	}

    @media only screen and (min-width: 768px){
        .logo{
            margin-left:5vw ;
			width: 138px ;
			margin-top: 3.5vh;
        }

		.logo:hover{
			background-color: white;
		}
        .burger{
            display: none;
        }

        nav{
            display: block;
            position: relative;
        }
		
        ul{
            margin: 0;
			margin-top: 3vh;
            flex-direction: row;
            gap: 90px;
        }

		a:hover{
			padding: 10px;
			background-color: var(--light);
			border-radius: 10px;
		}
        .dropdown{
            margin-inline: 2vw;
			background-color: white;
        }
    }
</style>
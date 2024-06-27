<script>
	import Card from '../components/card.svelte';
	import Search from '../components/search.svelte';
	import Qr from '../components/qr.svelte';
	import Logo from '../logo.png';

	const guests = [
		{
			name: 'Rebecca Ravnsborg Bjørklund',
			title: 'Brud',
			description: 'some description'
		},
		{
			name: 'Lasse Ravnsborg Bjørklund',
			title: 'Gom',
			description: 'some description'
		},
		{
			name: 'Rebecca Ravnsborg Bjørklund',
			title: 'Brud',
			description: 'some description'
		},
		{
			name: 'Rebecca Ravnsborg Bjørklund',
			title: 'Brud',
			description: 'some description'
		},
		{
			name: 'Rebecca Ravnsborg Bjørklund',
			title: 'Brud',
			description: 'some description'
		}
	];
</script>

<div class="navigation-container">
	<div class="logo-container">
		<div class="logo">
			<img src={Logo} alt="logo">
			<span class="logo-text"> Forever After </span>
		</div>
		<span class="seetingplan"> Bordplan </span>
	</div>
	<div class="search-container">
		<Search />
	</div>
	<div class="guests-container">
		{#each guests as guest}
			<Card name={guest.name} title={guest.title} description={guest.description} />
		{/each}
	</div>
	<div class="qr">
		<Qr />
	</div>
</div>

<style>
    :global(body) {
        margin: 0;
        padding: 0;
        background-color: #182b1f;
        font-family: Geist, serif;
    }

    .navigation-container {
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 15% 15% 50% 20%;
        padding: 0 2vw;
        height: 100vh;
        max-width: 25vw;
        border-right: 0.2px solid gray;
        overflow: hidden;
    }

    .logo-container {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }

    .logo {
        display: flex;
        flex-direction: column;
    }

    .logo img {
        height: 7em;
        width: 7em;
        padding: 0;
        margin: 0;
    }

    .logo-text {
        font-family: 'Savoye LET', Serif;
        font-size: 2em;
        background-image: -webkit-linear-gradient(-45deg,
        rgba(221, 184, 110, 1) 0%,
        rgba(187, 137, 61, 1) 20%,
        rgba(126, 87, 47, 1) 50%,
        rgba(204, 169, 98, 1) 80%,
        rgba(221, 184, 110, 1) 90%,
        rgba(221, 184, 110, 1) 100%);
        background-clip: text;
        -webkit-background-clip: text;
        text-fill-color: transparent;
        -webkit-text-fill-color: transparent;
    }

    .seetingplan {
        font-size: 4em;
        font-family: "Savoye LET", Serif;
        background-image: -webkit-linear-gradient(-45deg,
        rgba(221, 184, 110, 1) 0%,
        rgba(187, 137, 61, 1) 20%,
        rgba(126, 87, 47, 1) 50%,
        rgba(204, 169, 98, 1) 80%,
        rgba(221, 184, 110, 1) 90%,
        rgba(221, 184, 110, 1) 100%);
        background-clip: text;
        -webkit-background-clip: text;
        text-fill-color: transparent;
        -webkit-text-fill-color: transparent;
        padding-top: 2vh;
    }

    .search-container {
        display: flex;
        flex-direction: column;
        margin-top: 1em;
    }

    .guests-container {
        display: flex;
        flex-direction: column;
        gap: 2em;
        overflow: scroll;
        margin-bottom: 2vh;
    }

    .qr {
        height: 100%;
    }
</style>

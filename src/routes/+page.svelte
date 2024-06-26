<script>
	import Card from '../components/card.svelte';

	const guests = [{
		name: 'Rebecca Ravnsborg Bjørklund',
		title: 'Brud',
		description: 'some description'
	}, {
		name: 'Lasse Ravnsborg Bjørklund',
		title: 'Gom',
		description: 'some description'
	}];
</script>

<div class="navigation-container">
	<div class="logo">
		<div>LOGO</div>
	</div>
	<div class="search-container">
		<div>SEARCH</div>
	</div>
	<div class="guests-container">
		{#each guests as guest}
			<Card name={guest.name} title="Guest" description={guest.description} />
		{/each}
	</div>
</div>

<style>
    :global(body) {
        margin: 0;
        padding: 0;
        background-color: #182B1F;
    }

    .navigation-container {
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr 5fr;
        height: 100vh;
        max-width: 30vw;
        border-right: .5px solid white;
    }

    .search-container {
        display: flex;
        flex-direction: column;
    }

    .guests-container {
        display: flex;
        flex-direction: column;
        gap: 2em;
        padding: 0 2vw;

    }
</style>


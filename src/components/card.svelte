<script>
	export let name = 'name placeholder';
	export let title = 'short placeholder';
	export let description = 'short placeholder';
</script>

<div class="container">
	<div class="text-container">
		<h3>{name}</h3>
		<p class="title">Title</p>
		<p class="description">{title}</p>
	</div>
	<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" preserveAspectRatio="xMidYMin meet"
			 height="30"
			 width="30"
			 fill="currentColor">
		<path
			d="M16.1716 10.9999L10.8076 5.63589L12.2218 4.22168L20 11.9999L12.2218 19.778L10.8076 18.3638L16.1716 12.9999H4V10.9999H16.1716Z"></path>
	</svg>
</div>


<style>

    .container {
        /* Layout */
        display: flex;
        align-items: center;
        justify-content: space-between;

        /* Glass definition */
        background: rgba(255, 255, 255, 0.21);
        border-radius: 16px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        padding: 1vw;
        backdrop-filter: blur(11.5px);
        -webkit-backdrop-filter: blur(11.5px);

        /* Other */
        color: white;

    }

    .title {
        color: #999999;
        font-size: small;
        margin: 0;
        padding: 0;
    }

    .description {
        font-size: small;
        margin: 0;
        padding: .5em 0 0 0;
    }

    h3 {
        font-size: medium;
        padding: 0 0 1em 0;
        margin: 0;
    }
</style>
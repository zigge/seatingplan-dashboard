<script>
	export let name = 'name placeholder';
	export let title = 'short placeholder';
	export let description = 'short placeholder';
</script>

<div class="container">
	<div class="text-container">
		<h1>{name}</h1>
		<h4>Title</h4>
		<p>{title}</p>
	</div>
</div>


<style>
    .container {
        display: flex;
        background: rgba(255, 255, 255, 0.21);
        border-radius: 16px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        padding: 0 2vw;
        backdrop-filter: blur(11.5px);
        -webkit-backdrop-filter: blur(11.5px);
    }
</style>
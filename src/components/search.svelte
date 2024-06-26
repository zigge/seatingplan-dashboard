<script>

</script>

<div class="container">
	<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" preserveAspectRatio="xMidYMin meet"
			 height="20"
			 width="20"
			 fill="#FFFFFF">
		<path
			d="M18.031 16.6168L22.3137 20.8995L20.8995 22.3137L16.6168 18.031C15.0769 19.263 13.124 20 11 20C6.032 20 2 15.968 2 11C2 6.032 6.032 2 11 2C15.968 2 20 6.032 20 11C20 13.124 19.263 15.0769 18.031 16.6168ZM16.0247 15.8748C17.2475 14.6146 18 12.8956 18 11C18 7.1325 14.8675 4 11 4C7.1325 4 4 7.1325 4 11C4 14.8675 7.1325 18 11 18C12.8956 18 14.6146 17.2475 15.8748 16.0247L16.0247 15.8748Z"></path>
	</svg>
	<span class="separator"></span>
	<input id="search" placeholder="Søg person">

</div>


<style>
    .container {
        display: flex;
        padding: 1vw;
        align-items: center;
        background: rgba(255, 255, 255, 0.21);
        border-radius: 15px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        backdrop-filter: blur(11.5px);
        -webkit-backdrop-filter: blur(11.5px);
    }

    #search {
        width: 100%;
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box;
        height: 100%;
        background: none;
        outline: none;
        border: none;
        color: white;
    }

    .separator {
        width: 2px;
        height: 100%;
        border-left: 1px solid gray;
        margin-left: 10px;
        margin-right: 10px;
    }
</style>
<script>
	import { Html5Qrcode } from 'html5-qrcode';
	import { onMount } from 'svelte';


	onMount(() => {
		const html5QrCode = new Html5Qrcode('reader');
		const qrCodeSuccessCallback = (decodedText, decodedResult) => {

		};
		const config = { fps: 10, qrbox: { width: 250, height: 250 } };
		html5QrCode.stop();
		// html5QrCode.start({ facingMode: 'user' }, config, qrCodeSuccessCallback);

	});

</script>

<div id="reader"></div>

<style>
    #reader {
        height: 25vh;
        background-color: black;
    }
</style>
<script>
	import ScanQrCode from 'scan-qr-svelte/ScanQRCode.svelte';
	function handleMessage(event) {
		alert(event.detail.result);
	}
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
<ScanQrCode on:scanresult={handleMessage} />
<h1>Reuslt :</h1>

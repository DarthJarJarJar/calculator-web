<script>
    import Button from "./Button.svelte"
    $: num = "";
</script>
<div class="container">
    <br>

{#if num != "" }
<div class="input-num">{num}</div>
    {:else} <div id="invisible" class="input-num">-</div>
{/if}  
<br>
<Button bind:num/>
</div>	

<style>
    .input-num{
		background-color: #fff;
		width: 337px;
		margin: auto;
		text-align: right;
		border-radius: 1.5rem;
		padding: 10px;
		margin-bottom: 5px;
		height: 1.7cm;
		font-weight: bold;
		font-size: xx-large;
		word-wrap: break-word;
		inline-size: 337px;
		overflow-wrap: break-word;
		scroll-behavior: auto;
		overflow-x: scroll;
		  overflow-y: hidden;
	  white-space: nowrap;
	 
	 
	}
		
	#invisible {
		color: white;
	}
	
	.container {
		background-color: #3A3B3C;
		width: 400px;
		text-align: center;
		border-radius: 1.5rem;
		box-shadow: #D3D3D3;
	}
</style>
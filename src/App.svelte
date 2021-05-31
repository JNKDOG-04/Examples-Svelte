

<script>
	function playSound(number){
		const sound = new Audio();
		sound.src = 'assets/sounds/note'+ number +'.wav';
		sound.load();
		sound.play();
	}
</script>

<main>
	<h1 class="title">Piano</h1>
	<div class="row">
		<div class="col-lg-6">
			<div class="list-group">
				<div on:click={ () => playSound(1) } class="list-group-item list-group-item-action bg-primary ">DO</div>
				<div on:click={ () => playSound(2) } class="list-group-item list-group-item-action bg-info">RE</div>
				<div on:click={ () => playSound(3) } class="list-group-item list-group-item-action bg-primary">MI</div>
				<div on:click={ () => playSound(4) } class="list-group-item list-group-item-action bg-info">FA</div>
				<div on:click={ () => playSound(5) } class="list-group-item list-group-item-action bg-primary">SOL</div>
				<div on:click={ () => playSound(6) } class="list-group-item list-group-item-action bg-info">LA</div>
				<div on:click={ () => playSound(7) } class="list-group-item list-group-item-action bg-primary">SI</div>
				<div on:click={ () => playSound(1) } class="list-group-item list-group-item-action bg-info">DO#</div>
			</div>
		</div>
	</div>
</main>

<style>
	.title{
		display: flex;
		justify-content: center;
		align-items: center;
		color: #48CAE4;
		font-size: 45px;
		margin-bottom: 45px;
	}

	.list-group-item{
		cursor:pointer;
		height: 50px;
	}

	.row{
		display: flex;
		justify-content: center;
		align-items: center;
		height: 90vh;
	}

	.list-group-item:active{
		opacity: .50;
	}

	main{
		background-color: #03045E;
	}
</style>
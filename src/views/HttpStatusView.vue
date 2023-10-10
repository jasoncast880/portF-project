<template>
	<div class = "bckgrnd-containter">
		<div class = "content">
			<h1>Hello Neobrualism</h1>
			<p>Content Content Content</p>
		</div>
	</div>
</template>
<style scoped>
	.bckgrnd-container {
		position:relative;
		background-color: #f7f7f7;
		padding: 20px;
	}

	.bckgrnd-container::before,
	.bckgrnd-container::after {
		content: "";
		position: absolute;
		width:100%;
		height: 2px;
		background-color: #333;
	}
	.bckgrnd-container::before {
		top: 50%;
		transform: translateY(-50%);
	}
	.bckgrnd-container::after{
		bottom:50%;
		transform: translateY(50%);
	}
</style>

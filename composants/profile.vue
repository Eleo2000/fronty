


<template>
	<div>
		

		<div class="Profil-mini">
			<div class="quit-pro cursor-h">fermer</div>
			<div class="img-pro"><div class="imgXd"></div></div>
			<div class="info-pro pad-pro">
				<div class="name-pro">name Profile</div>
				<div class="status-pro">status Profile</div>
			</div>
			<div class="gest-pro pad-pro">
				<div class="param-pro link-l cursor-h">parametre Profile</div>
				<div class="deconnexion-pro link-l  cursor-h">deconnexion Profile</div>
			</div>

		</div>
	</div>
</template>

<style>
.Profil-mini {
	position:relative;
	display: grid;
	justify-items: center;
	padding-top: 16px;
	padding-bottom: 16px;
	border: 1px solid black;
	width: 300px;
}

.quit-pro{
	position: absolute;
	top: 0;
	margin-top: 8px;
	right: 16px;
}

.imgXd{
	display: grid;
	align-self: center;
	justify-content: center;
	align-content: center;
	justify-self: center;
	align-items: center;
	justify-items: center;
	width: 40px;
	height: 40px;
	border-radius: 40px;
	background-color: red;
}
.imgXd::before{
	z-index: -1;
	display: grid;
	content: "";
	width: 50px;
	height: 50px;
	border: 1px solid black;
	border-radius: 40px;
	background-color: rgb(255, 255, 255);
}
.img-pro{
	display: grid;
	position: relative;
	height: 100%;
	width: 100%;
	justify-items: center;
	align-items: center;
}
.img-pro::before{
	z-index: -1;
	display: grid;
	position: absolute;
	content: "";
	height: 1px;
	width: 70%;
	background-color: red;
}



.pad-pro{
	padding-top: 24px;
}

.info-pro{
	display: grid;
	justify-self: baseline;
	padding-left: 24px;
	
}

.name-pro{
	padding-bottom: 8px
}
.gest-pro{
	display: grid;
	grid-template-columns: 1fr 1fr;
}

.link-l:hover{
	
	text-decoration: underline;
}

.cursor-h{
	cursor: pointer;
}


</style>

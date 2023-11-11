


<template>
	<div>
		
		<div class="cont-carda">
			<div class="card ">
			<div class="card-image">image</div>
			<div class="bot">
				<div class="prof-carda">
					<div class="prop-carda">
						<div class="ico-prof"></div>
						<div class="name-carda">namesddddddddddddddddddddd </div>
					</div>
					<div class="cat-carda">categorysdsdsdsdsdsdsssasas</div>
				</div>
				<div class="stat-carda">
					<div class="view-carda">3 vues</div>
					<div class="star-carda">4 stars</div>
				</div>
			</div>
		</div>
		<div class="card ">
			<div class="card-image">image</div>
			<div class="bot">
				<div class="prof-carda">
					<div class="prop-carda">
						<div class="ico-prof"></div>
						<div class="name-carda">namesddddddddddddddddddddd </div>
					</div>
					<div class="cat-carda">categorysdsdsdsdsdsdsssasas</div>
				</div>
				<div class="stat-carda">
					<div class="view-carda">3 vues</div>
					<div class="star-carda">4 stars</div>
				</div>
			</div>
		</div>
		<div class="card ">
			<div class="card-image">image</div>
			<div class="bot">
				<div class="prof-carda">
					<div class="prop-carda">
						<div class="ico-prof"></div>
						<div class="name-carda">namesddddddddddddddddddddd </div>
					</div>
					<div class="cat-carda">categorysdsdsdsdsdsdsssasas</div>
				</div>
				<div class="stat-carda">
					<div class="view-carda">3 vues</div>
					<div class="star-carda">4 stars</div>
				</div>
			</div>
		</div>
		<div class="card ">
			<div class="card-image">image</div>
			<div class="bot">
				<div class="prof-carda">
					<div class="prop-carda">
						<div class="ico-prof"></div>
						<div class="name-carda">namesddddddddddddddddddddd </div>
					</div>
					<div class="cat-carda">categorysdsdsdsdsdsdsssasas</div>
				</div>
				<div class="stat-carda">
					<div class="view-carda">3 vues</div>
					<div class="star-carda">4 stars</div>
				</div>
			</div>
		</div>
		</div>
		
	</div>
</template>

<style>

.cont-carda{
	display: grid;
	grid-template-columns:  repeat(auto-fit, minmax(210px, 1fr));
	grid-gap: 24px;
	justify-items: center;
}

.card {

	border: 1px solid rgba(255, 255, 255, 0);
	box-shadow: 0px 2px 6px #0000002e;
	width: 100%;
	max-width: 280px;
	height: 210px;
	display: grid;
	min-width: 210px;
	grid-template-rows: 1fr 0.2fr;
	padding-bottom: 8px;

}

.prop-carda{
	display: grid;
	grid-template-columns: max-content 1fr;
	
	align-items: center;
}

.card:hover {

	border: 1px solid #957737;
	box-shadow: 0px 4px 6px #0000002e;



}

.card-image {
	background-color: #957737;
}

.bot {
	border-top: 1px solid #957737;
	display: grid;
	grid-template-columns: 1fr 1fr;
	padding-top: 4px;
	padding-left: 12px;
	align-items: center;

}

.name-carda,
.cat-carda,
.ico-prof {
	text-overflow: ellipsis;
	overflow: hidden;
	white-space: nowrap;
	width: 100px;

} .ico-prof{
	margin-right:8px;
	width: max-content;
	width: 32px;
    height: 32px;
    background: red;
    border-radius: 50%;

}


.stat-carda {
	display: grid;
	justify-content: center;
}
</style>

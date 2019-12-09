<template>
	<div class="projects">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Projects</template>

			<hr class="my-4" />

			<div id="content">
				<b-card></b-card>
				<b-card></b-card>
				<b-card></b-card>
				<b-card></b-card>
				<b-card></b-card>
			</div>
		</b-jumbotron>
	</div>
</template>

<script>
export default {
	name: "Projects"
};
</script>

<style>
.projects {
	padding-top: 10px;
}

#content {
	background-color: mintcream;
	border-radius: 5px;
}
</style>
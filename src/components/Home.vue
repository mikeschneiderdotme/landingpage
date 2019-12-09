<template>
	<div class="home">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Welcome</template>

			<template
				v-slot:lead
			>To the landing page for software developer and data specialist Michael Schneider.</template>

			<hr class="my-4" />

			<div id="content">
				<b-tabs content-class="mt-3" align="center" fill>
					<b-tab title="Contact Info" active>
						<p>Contact Info</p>
					</b-tab>
					<b-tab title="Skills">
						<p>Skills</p>
					</b-tab>
					<b-tab title="Job History">
						<p>Job History</p>
					</b-tab>
					<b-tab title="Awards">
						<p>Awards</p>
					</b-tab>
				</b-tabs>
			</div>
		</b-jumbotron>
	</div>
</template>

<script>
export default {
	name: "Home"
};
</script>

<style lang="scss">
#content {
	background-color: mintcream;
}

ul.nav-tabs {
	background-color: mediumseagreen;
}

a {
	color: white;
}

.tab-pane {
	color: black;
}
</style>
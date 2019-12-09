<template>
	<div class="home">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Welcome</template>

			<template
				v-slot:lead
			>To the landing page for software developer and database specialist Michael Schneider.</template>

			<hr class="my-4" />

			<div id="content">
				<b-tabs content-class="mt-3" align="center" fill>
					<b-tab no-body title="Contact Info" active>
						<p>Contact Info email, phone, address, linkedin, github</p>
					</b-tab>
					<b-tab title="About">
						<p>List about me Name, Occupation, Image, Description</p>
					</b-tab>
					<b-tab no-body title="Resume">
						<b-card-img bottom :src="require('../assets/Resume.png')"></b-card-img>
					</b-tab>
					<b-tab no-body title="Cover Letter">
						<b-card-img bottom :src="require('../assets/CoverLetter.png')"></b-card-img>
					</b-tab>
				</b-tabs>
			</div>
		</b-jumbotron>
	</div>
</template>

<script>
export default {
	name: "Home",
	components: {},
	data() {
		return {};
	}
};
</script>

<style lang="scss">
#content {
	background-color: mintcream;
}

ul.nav-tabs {
	background-color: mediumseagreen;
}

a.nav-link {
	color: white;
}

.tab-pane {
	color: black;
}
</style>
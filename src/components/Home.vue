<template>
	<div class="home">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Welcome</template>

			<template
				v-slot:lead
			>To the landing page for software developer and database specialist Michael Schneider.</template>

			<hr class="my-4" />

			<div id="content">
				<b-tabs
					content-class="mt-3"
					align="center"
					style="min-height: 500px; border: 2px solid lightblue; border-radius: 5px"
					fill
				>
					<b-tab no-body title="Contact Info" active>
						<b-container fluid>
							<b-row>
								<b-col style="padding-bottom: 15px;">
									<b-card title="Email" style="max-height:125px;">
										<b-card-text>mschneider2628@gmail.com</b-card-text>
									</b-card>
									<b-card title="Phone" style="max-height:125px;">
										<b-card-text>(715)432-9101</b-card-text>
									</b-card>
									<b-card title="LinkedIn" style="max-height:125px;">
										<b-button
											variant="primary"
											href="https://www.linkedin.com/in/michael-schneider-145250141/"
										>To LinkedIn</b-button>
									</b-card>
									<b-card title="Github" style="max-height:125px;">
										<b-button href="https://github.com/Cellor425">To Github</b-button>
									</b-card>
								</b-col>
							</b-row>
						</b-container>
					</b-tab>
					<b-tab title="About">
						<b-container fluid>
							<b-row>
								<b-col style="max-width: 300px; margin: auto">
									<b-img :src="require('../assets/profile pic.jpg')" fluid></b-img>
								</b-col>
							</b-row>
							<b-row>
								<b-col>
									<b-card title="About Me">
										<b-card-text>
											Experienced Team Trainer with a demonstrated history of working in the
											retail industry. Extensive experience in working with computer hardware. Skills
											in several programming languages such as C#, JavaScript, Java, and T-SQL.
											Experience in database creation, design, and management as well as program creation
											and user design. Experience in frameworks such as .NET Core, .NET Framework, Vue.js,
											and Flask(python).
										</b-card-text>
									</b-card>
								</b-col>
							</b-row>
						</b-container>
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
.home {
	padding-top: 10px;
}

#content {
	background-color: mintcream;
	border-radius: 5px;
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
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
						<b-container fluid style="max-width: 600px;">
							<b-row>
								<b-col style="padding-bottom: 15px;">
									<b-card title="Email" style="max-height:125px;">
										<b-card-text>mschneider2628@gmail.com</b-card-text>
									</b-card>
									<b-card title="Phone" style="max-height:125px;">
										<b-card-text>(715)432-9101</b-card-text>
									</b-card>
									<b-card style="max-height:125px;">
										<b-link href="https://www.linkedin.com/in/michael-schneider-145250141/">
											<b-img src="../assets/linkedin.png" style="max-height: 40px;"></b-img>
										</b-link>
										<p></p>
										<b-link href="https://github.com/Cellor425">
											<b-img src="../assets/github.png" style="max-height: 35px;"></b-img>
										</b-link>
									</b-card>
								</b-col>
							</b-row>
						</b-container>
					</b-tab>
					<b-tab title="About">
						<b-container fluid>
							<b-row>
								<b-col style="max-width: 300px; margin: auto">
									<b-img src="../assets/profile pic.jpg" fluid></b-img>
								</b-col>
							</b-row>
							<b-row>
								<b-col>
									<b-card title="About Me" style="max-width: 600px; margin: auto;">
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
						<!-- File_Id = 1GYQjrvCGHBvwQkeFoc1WO2fHwS_gOn5ydX4TLVBJtXQ -->
						<b-button
							href="https://docs.google.com/document/d/1GYQjrvCGHBvwQkeFoc1WO2fHwS_gOn5ydX4TLVBJtXQ/export?format=pdf"
							size="sm"
						>Download PDF</b-button>
						<b-embed
							type="iframe"
							aspect="4by3"
							src="https://docs.google.com/document/d/e/2PACX-1vQWL_Pfkyn3nG6RB-Gbt6JU_uq89_vDZQvzTtmSHCU9W5ca2wYRoSF3gdHTgu-NLpDYgNp7xF3qiHs7/pub?embedded=true"
						></b-embed>
					</b-tab>
					<b-tab no-body title="Cover Letter">
						<!-- Fild_Id = https://docs.google.com/document/d/1eZJARijNZgjgud4gAIJQ4eWZIT5KgEwfSExhFnkmI7I/edit?usp=sharing -->
						<b-button
							href="https://docs.google.com/document/d/1eZJARijNZgjgud4gAIJQ4eWZIT5KgEwfSExhFnkmI7I/export?format=pdf"
							size="sm"
						>Download PDF</b-button>
						<b-embed
							type="iframe"
							aspect="4by3"
							src="https://docs.google.com/document/d/e/2PACX-1vSIWFJRc8tfn0mEeaGk1jSQGWSnmHc_kXuMD4AN3eICN7e415UFbkgTlsRdFW-RMJ8lAiamyeZm1Fnm/pub?embedded=true"
						></b-embed>
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
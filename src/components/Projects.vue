<template>
	<div class="projects">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Projects</template>

			<hr class="my-4" />

			<div id="content">
				<b-card>
					<!-- Pizza Maker WPF Card -->
					<h5 class="mt-0">
						<b-badge id="padding" variant="success">Complete</b-badge>Pizza Maker WPF
					</h5>
					<b-badge id="padding">C#</b-badge>
					<b-badge id="padding">WPF</b-badge>
					<p>A simple WPF application to demonstrate the use of multiple OOP design patterns.</p>

					<b-button v-b-toggle="'pizza'">Project Details</b-button>
					<b-link href="https://github.com/Cellor425/Pizza-Maker-Program-2018-OOP-Design">
						<b-img src="../assets/github.png" style="max-height: 25px; padding-left: 5px;"></b-img>
					</b-link>
					<b-collapse id="pizza" class="mt-2">
						<b-card>
							<b-button id="padding" v-b-toggle="'class-diagram-pizza'" size="sm">Class Diagram</b-button>
							<b-button id="padding" v-b-toggle="'info-pizza'" size="sm">Technical Information</b-button>
							<b-collapse id="class-diagram-pizza" class="mt-2">
								<b-img src="../assets/PizzaMaker.png" style="width: 100%; border: 1px solid black;"></b-img>
							</b-collapse>
							<b-collapse id="info-pizza" class="mt-2">
								<h6>Explaination</h6>
								<p>
									The Pizza Maker application is a program that allows a user to create a custom pizza
									with multiple ingredients from putting the pizza together to cooking the pizza and finalizing
									the pizza for pickup.
								</p>
								<p>
									The application has three main parts that contribute to the whole: the pizza states, the
									ingredients, and the pizza objects. The pizza states handle the changing of the pizza as it
									is built and cooked. The ingredients are objects that can be added to the pizza object. The pizza
									objects are the glue that holds the ingredients and state information as well as a template to calculate
									the total cost of the pizza when all is said and done.
								</p>
								<p>
									The WPF application attached is a crude, yet effective, way to test some of the functionality of
									the program. The window has 3 buttons, and each button tests a different design pattern in the program.
									The create button creates the pizza for the user. The add ingredients button adds the ingredients for a basic
									pepperoni pizza, and the process button moves the pizza through the different states from unfinished to cooked and
									then final.
								</p>
								<h6>Design Patterns</h6>
								<p>
									The three design patterns I chose to use in this project are the state, template,
									and factory patterns. The factory pattern is implemented into the creation of ingredients and
									pizza objects with the use of two separate factory classes. The state pattern is implemented
									to track the stage of the pizza making process that the pizza object is in. The template pattern
									is implemented in the pizza objects and handles the calculation of the cost of the pizza object.
								</p>
								<h6>Possible Alternative</h6>
								<p>
									A possible alternative to using the template pattern and factory pattern could be the use of
									the decorator pattern to wrap the ingredients of the pizza onto the pizza object. In place
									of the state pattern, an observer pattern could have been implemented to update the pizza when
									it is moved through the making process.
								</p>
							</b-collapse>
						</b-card>
					</b-collapse>
				</b-card>

				<!-- Media Monkey Card -->
				<b-card>
					<h5 class="mt-0">
						<b-badge id="padding" variant="success">Complete</b-badge>Media Monkey
					</h5>
					<b-badge id="padding">C#</b-badge>
					<b-badge id="padding">JavaScript</b-badge>
					<b-badge id="padding">.NET Core</b-badge>
					<b-badge id="padding">Node.js</b-badge>
					<b-badge id="padding">FTP</b-badge>
					<p>A .NET Core MVC web application developed over 3 months with a team of 3 developers.</p>
					<b-button v-b-toggle="'mediamonkey'">Project Details</b-button>
					<b-link href="https://github.com/Cellor425/MM">
						<b-img src="../assets/github.png" style="max-height: 25px; padding-left: 5px;"></b-img>
					</b-link>
					<b-collapse id="mediamonkey" class="mt-2">
						<b-card>
							<b-button
								id="padding"
								href="https://mediamonkey.mjschneider1.com/"
								style="background-color: orange; color: black;"
								size="sm"
							>To Media Monkey</b-button>
							<b-button id="padding" v-b-toggle="'mm-inner-1'" size="sm">Site Logo</b-button>
							<b-button id="padding" v-b-toggle="'mm-inner-2'" size="sm">Description</b-button>
							<b-collapse id="mm-inner-1" class="mt-2">
								<b-img src="../assets/Logo.png" style="max-width:300px; border: 1px solid black;"></b-img>
							</b-collapse>
							<b-collapse id="mm-inner-2" class="mt-2">
								<h6>Project Objective</h6>
								<p>
									The objective of this project was to make a video hosting and sharing platform that would allow users
									to create a profile, upload and manage videos, comment on videos, and search for specific videos.
								</p>
								<h6>Process and Technologies</h6>
								<p>
									We were given 15 weeks, which consisted of five 3 week sprint cycles, to complete development and deliver a final product.
									The goal for each sprint was to develop a core piece of functionality for the website such as video upload and profile creation.
									The main framework that the project was built on is ASP.NET Core 2.1 which connected to a remote MSSQL database on the backend and
									served pages using Razor syntax.
								</p>
								<h6>My Role</h6>
								<p>
									I was given the role of business logic tier developer, however, I contributed in each part of the project stack from backend mangement to front end design.
									The main functionalities that I worked on was the features around the handling on video files. This involved allowing a user to upload a video
									file and store it on a remote FTP server as well as creating database records connected to that file. As stated the method I chose to handle video file storage
									as through an FTP server in which the file location was stored in the database with related information.
								</p>
							</b-collapse>
						</b-card>
					</b-collapse>
				</b-card>

				<!-- Backup Saves Console Card -->
				<b-card>
					<h5 class="mt-0">
						<b-badge id="padding" variant="warning">In Dev</b-badge>Backup Saves Console
					</h5>
					<b-badge id="padding">C#</b-badge>
					<b-badge id="padding">.NET Framework</b-badge>
					<b-link href="https://github.com/Cellor425/BackupSaves">
						<b-img src="../assets/github.png" style="max-height: 25px; padding-left: 5px;"></b-img>
					</b-link>
					<p>A .NET Framework console application to backup remote save files to a new location.</p>
					<b-button v-b-toggle="'backup'">Project Details</b-button>
					<b-collapse id="backup" class="mt-2">
						<b-card>
							<h6>Description</h6>
							<p>Make a description idiot</p>
						</b-card>
					</b-collapse>
				</b-card>

				<!-- Landing Page Card -->
				<b-card>
					<h5 class="mt-0">
						<b-badge id="padding" variant="warning">In Dev</b-badge>Landing Page
					</h5>
					<b-badge id="padding">JavaScript</b-badge>
					<b-badge id="padding">Vue CLI</b-badge>
					<p>A .NET Framework console application to backup remote save files to a new location.</p>
					<b-button v-b-toggle="'landing'">Project Details</b-button>
					<b-link href="https://github.com/Cellor425/landingpage">
						<b-img src="../assets/github.png" style="max-height: 25px; padding-left: 5px;"></b-img>
					</b-link>
					<b-collapse id="landing">
						<b-card>
							<h6>Description</h6>
							<p>Make a description idiot</p>
						</b-card>
					</b-collapse>
				</b-card>
			</div>
		</b-jumbotron>
	</div>
</template>

<script>
export default {
	name: "Projects",
	components: {}
};
</script>

<style>
.projects {
	padding-top: 10px;
}

#content {
	background-color: mintcream;
	color: black;
	border-radius: 5px;
}

#padding {
	margin: 0 1px 0 1px;
}
</style>
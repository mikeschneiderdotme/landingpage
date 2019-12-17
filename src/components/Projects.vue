<template>
	<div class="projects">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Projects</template>

			<hr class="my-4" />

			<div id="content">
				<b-card>
					<!-- Pizza Maker WPF Card -->
					<h5 class="mt-0">
						<b-badge id="padding" variant="success">Dev Ended</b-badge>Pizza Maker WPF
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
						<b-badge id="padding" variant="success">Dev Ended</b-badge>Media Monkey
					</h5>
					<b-badge id="padding">C#</b-badge>
					<b-badge id="padding">JavaScript</b-badge>
					<b-badge id="padding">.NET Core</b-badge>
					<b-badge id="padding">Entity Framework</b-badge>
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
					<p>A .NET Framework console application to backup remote save files to a new location.</p>
					<b-button v-b-toggle="'backup'">Project Details</b-button>
					<b-link href="https://github.com/Cellor425/BackupSaves">
						<b-img src="../assets/github.png" style="max-height: 25px; padding-left: 5px;"></b-img>
					</b-link>
					<b-collapse id="backup" class="mt-2">
						<b-card>
							<h6>Description</h6>
							<p>
								The project started as a simple console app to grab remote save files from my steam and uplay games and store them in
								an alternate local location. I wanted to do this because I had recently lost all my "cloud" saves when I reset my
								windows install and the cloud backups didnt make it.
							</p>
							<p>
								The program contains a simple input menu and single key command interface that allows a user to run the saves,
								reset the window, and exit the application. In it's current state the application has an api utility that accesses the
								steam api service to get my owned game ids and runs a directory copy with robust error handling and logging. Once complete,
								the backup returns a summary to the window.
							</p>
							<h6>Technologies</h6>
							<p>
								For this project, I needed use of windows file manipulation which needed .NET Framework. I usually like to use .NET Core for
								the cross platform support. I made the program in Visual Studio 2019 and includes the use of the Newtonsoft.Json nuget package
								for deserializing the request to the steam api server.
							</p>
							<h6>Future Developmment</h6>
							<p>
								Future development for the project would be to include a config file so that onther users can input their steam id and modify the location
								for backups or if their steam and uplay are installed in different locations on their machines. I would also like to clean up the error checking
								as it currently counts games that I don't have saves for as errors in the backup process. This includes a better summary in the console window. I
								would also like to add more robust commands to the console for my functionality such as listing your games, backing up a single game, ect.
							</p>
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
							<p>
								This project was about making a SAP(Single Page Applicaiton) using a popular front end framework so that I had a centralized location
								to promote myself as a developer from. Initially I was going to use React for the front end but decided I didn't
								need the overcomplexity it brings and so Vue was what I went with.
							</p>
							<p>
								The website contains two main component views: Home and Projects. The home component has a tab structure with a quick view
								of my resume and cover letter, as well as, links to my work and how users can contact me. The project page has a detailed
								list of some, but not all, of my projects I have worked on over the years.
							</p>
							<h6>Technologies</h6>
							<p>
								As stated in the description, I used Vue CLI to generate the scaffolding for my SAP. I also made heavy use of the Bootstrap-Vue package
								in my components so that I could get a respectable looking page up quickly.
							</p>
							<h6>Future Developmment</h6>
							<p>
								Future additions to the page will include a way for users to reach me through the site via form submission of some sort, and for users to be able to download
								a PDF version of my resume and cover letter if users want. I also want to make the project cards reusable so I can add more of my projects. Also a way to filter
								and search the projects would be nice.
							</p>
						</b-card>
					</b-collapse>
				</b-card>

				<!-- Capstone Card -->
				<b-card>
					<h5 class="mt-0">
						<b-badge id="padding" variant="primary">Contributed</b-badge>Syllabus Editor/Course Commons
					</h5>
					<b-badge id="padding">C#</b-badge>
					<b-badge id="padding">.NET Framework</b-badge>
					<b-badge id="padding">Entity Framework</b-badge>
					<p>The suite of applications that my team worked on for a capstone project at NTC.</p>
					<b-button v-b-toggle="'capstone'">Project Details</b-button>
					<b-collapse id="capstone">
						<b-card>
							<h6>Description</h6>
							<p>
								The syllabus editor is a .NET Framework MVC application that utilizes an API (Course Commons) that contains data used across multiple applications
								and an application specific database managed with entity framework. The application allows instructors to log in with their credentials and manage
								syllabi for the sections they are assigned to. The editor also uses .NET user identity and role based authentication that is used to manage access to
								different parts of the application and store a unique identifier for the instructor accessing the application.
							</p>
							<p>
								The course commons contains several applications that interact with a database containing records that are used in multiple NTC projects. The commons
								applications include the dashboard, api, and adapter framework. The dashboard is the GUI component for the api which serves up data from the course commons
								database. The adapter framework is a class library containing the models and utilities needed to interact with the api and is used in the syllabus editor and
								dashboard.
							</p>
							<h6>My Contribution</h6>
							<p>
								Out team was tasked with bringing the syllabus editor application back to a working state after the overhaul of the backend data that resulted in the creation of
								the course commons api. A lot of the work done to the project was in an effort to make sure the "frankenstein" melding of two data sources would result in usable models
								for the application views.
							</p>
							<p>
								We overhauled the population of the application specific database so that it was able to link to matching records form the api. Then we spent a large
								amount of time trying to get an overly complex model wrapper to reference data from the api correctly. The wrapper made heavy use of generics and repository pattern and after
								3 sprints of working on it we decided to remove it in favor of a view model approach.
							</p>
							<p>
								The view models removed any direct data referencing to the api in favor of using models that would be populated by api data and a syllabus specific model object in the controller
								actions. This ment that the syllabus models used were drastically simplified and the api data was no longer referenced in the editor outside of controller actions. This has
								the added benefit of having a clear seperation of the api from the application which would prevent bugs from being introduced from development on either project that would change the
								relationship between them.
							</p>
							<!--<h6>Lessons Learned</h6>
							<p>Put something here idiot.</p>-->
						</b-card>
					</b-collapse>
				</b-card>

				<!-- Data Analytics -->
				<b-card>
					<h5 class="mt-0">
						<b-badge id="padding" variant="success">Complete</b-badge>Technology Survey Analysis
					</h5>
					<b-badge id="padding">SQL</b-badge>
					<b-badge id="padding">MongoDB</b-badge>
					<b-badge id="padding">R</b-badge>
					<b-badge id="padding">Tableau</b-badge>
					<p>An analysis of data collected about technology used by people. Sample size of 150 people.</p>
					<b-button v-b-toggle="'analytics'">Project Details</b-button>
					<b-collapse id="analytics">
						<b-card>
							<b-button
								href="https://docs.google.com/document/d/1Fm1vV60z8V89O5O6AeFOXKYOvXgeG1oY/export?format=pdf"
								size="sm"
							>Download PDF</b-button>
							<b-embed
								type="iframe"
								aspect="4by3"
								src="https://docs.google.com/document/d/e/2PACX-1vT9rFmzmoilSCSpG4egvm3j7R3trBdi3Dy02zJeU9pftgsSFOUdHCDyWTMwX-Bqaw/pub?embedded=true"
							></b-embed>
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
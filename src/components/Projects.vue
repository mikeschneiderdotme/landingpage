<template>
	<div class="projects">
		<b-jumbotron bg-variant="info" text-variant="white">
			<template v-slot:header>Projects</template>

			<hr class="my-4" />

			<div id="content">
				<b-card>
					<h5 class="mt-0">
						Pizza Maker WPF
						<b-badge>C#</b-badge>
						<b-badge>WPF</b-badge>
					</h5>
					<p>A simple WPF application to demonstrate the use of multiple OOP design patterns.</p>

					<b-button v-b-toggle="'pizza'">Project Details</b-button>
					<b-collapse id="pizza" class="mt-2">
						<b-card>
							<b-button v-b-toggle="'class-diagram-pizza'" size="sm">Class Diagram</b-button>
							<b-collapse id="class-diagram-pizza" class="mt-2">
								<b-img src="../assets/PizzaMaker.png" style="width: 100%; border: 1px solid black;"></b-img>
							</b-collapse>
							<b-button v-b-toggle="'info-pizza'" size="sm">Techincal Information</b-button>
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
				<b-card>
					<h5 class="mt-0">
						Media Monkey
						<b-badge>C#</b-badge>
						<b-badge>JavaScript</b-badge>
						<b-badge>Razor</b-badge>
						<b-badge>.NET Core</b-badge>
						<b-badge>Node.js</b-badge>
					</h5>
					<p>A simple WPF application to demonstrate the use of multiple OOP design patterns.</p>
					<b-button v-b-toggle="'mediamonkey'">Project Details</b-button>
					<b-collapse id="mediamonkey" class="mt-2">
						<b-card>
							<b-button v-b-toggle="'mm-inner-1'" size="sm">Site Logo</b-button>
							<b-collapse id="mm-inner-1" class="mt-2">
								<b-img src="../assets/Logo.png" style="max-width:300px; border: 1px solid black;"></b-img>
							</b-collapse>
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
</style>
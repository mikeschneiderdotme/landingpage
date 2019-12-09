<template>
	<div id="app">
		<header>
			<b-navbar toggleable="lg" type="light" sticky="true">
				<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
				<b-navbar-brand to="/">Michael Schneider</b-navbar-brand>
				<b-collapse id="nav-collapse" is-nav>
					<b-navbar-nav>
						<b-nav-item>
							<b-link to="/projects" router-tag="li">Projects</b-link>
						</b-nav-item>
					</b-navbar-nav>
				</b-collapse>
			</b-navbar>
		</header>
		<div class="container">
			<router-view />
		</div>
		<footer>
			<div class="w-auto p-3 fixed-bottom">Michael Schneider's Portfolio &copy;2019</div>
		</footer>
	</div>
</template>

<script>
export default {
	name: "app",
	components: {}
};
</script>

<style lang="scss">
@import "~bootstrap/dist/css/bootstrap.css";
@import "~bootstrap-vue/dist/bootstrap-vue.css";

body {
	background-color: mintcream !important;
	min-height: 300px;
}

.navbar {
	background-color: mediumseagreen;
	font-size: 125%;
}

a.navbar-brand {
	font-size: 125%;
}

div.fixed-bottom {
	background-color: mediumseagreen;
	text-align: center;
}
</style>
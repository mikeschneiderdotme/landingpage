<template>
	<div id="app">
		<b-navbar toggleable="lg" type="dark" sticky="true">
			<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
			<b-navbar-brand to="/">Michael Schneider</b-navbar-brand>
			<b-collapse id="nav-collapse" is-nav>
				<b-navbar-nav>
					<b-nav-item>
						<b-link to="/about" router-tag="li">About</b-link>
					</b-nav-item>
					<b-nav-item>
						<b-link to="/projects" router-tag="li">Projects</b-link>
					</b-nav-item>
				</b-navbar-nav>
			</b-collapse>
		</b-navbar>
		<router-view />
	</div>
</template>

<script>
export default {
	name: "app",
	components: {}
};
</script>

<style>
body {
	background-color: beige;
}

.navbar {
	background-color: olive;
}
</style>
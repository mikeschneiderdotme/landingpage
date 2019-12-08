<template>
	<div class="hello">
		<div class="holder">
			<form @submit.prevent="addSkill">
				<ValidationProvider rules="min" v-slot="{ errors }">
					<input type="text" placeholder="Enter a skill you have.." v-model="skill" />
					<transition
						name="alert-in"
						enter-active-class="animated flipInX"
						leave-active-class="animated flipOutX"
					>
						<p class="alert" v-if="errors.length > 0">{{ errors[0] }}</p>
					</transition>
				</ValidationProvider>
			</form>
			<ul>
				<transition-group
					name="list"
					enter-active-class="animated bounceInUp"
					leave-active-class="animated bounceOutDown"
				>
					<li v-for="(data, index) in skills" :key="index + 0">
						{{data.skill}}
						<i class="fa fa-minus-circle" v-on:click="remove(index)"></i>
					</li>
				</transition-group>
			</ul>

			<p>These are the skills that you possess.</p>
		</div>
	</div>
</template>

<script>
import { ValidationProvider, extend, validate } from "vee-validate";

extend("min", value => {
	return value.length >= 5;
});

export default {
	name: "Skills",
	components: { ValidationProvider },
	data() {
		return {
			skill: "",
			skills: [{ skill: "Vue.js" }, { skill: "Frontend Developer" }]
		};
	},
	methods: {
		addSkill() {
			validate(this.skill, "min").then(result => {
				if (result.valid) {
					this.skills.push({ skill: this.skill });
					this.skill = "";
				} else {
					console.warn("Not valid");
				}
			});
			/*eslint no-console: ["error", { allow: ["warn", "error"] }] */
		},
		remove(id) {
			this.skills.splice(id, 1);
		}
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import "https://maxcdn.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css";
@import "https://cdn.jsdelivr.net/npm/animate.css@3.5.1";

.alert-in-enter-active {
	animation: bounce-in 0.5s;
}

.alert-in-leave-active {
	animation: bounce-in 0.5s reverse;
}

@keyframes bounce-in {
	0% {
		transform: scale(0);
	}
	50% {
		transform: scale(1.5);
	}
	100% {
		transform: scale(1);
	}
}

.holder {
	background: #fff;
}

.alert {
	background: #fdf2ce;
	font-weight: bold;
	display: inline-block;
	padding: 5px;
	margin-top: -20px;
}

input {
	width: calc(100% - 40px);
	border: 0;
	padding: 20px;
	font-size: 1.3em;
	background-color: #323333;
	color: #687f7f;
}

ul {
	margin: 0;
	padding: 0;
	list-style-type: none;
}

ul li {
	padding: 20px;
	font-size: 1.3em;
	background-color: #e0edf4;
	border-left: 5px solid #3eb3f6;
	margin-bottom: 2px;
	color: #3e5252;
}

p {
	text-align: center;
	padding: 30px 0;
	color: gray;
}

.container {
	box-shadow: 0px 0px 40px lightgray;
}
</style>

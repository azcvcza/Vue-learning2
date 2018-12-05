<template>
	<form @submit="addMessage">
		<div class="form-group">
			<input
				class="form-control"
				v-model="newMessage.title"
				maxlength="40"
				autofocus
				placeholder="Pleaseintroduce yourself :)"
			>
		</div>
		<div class="form-group">
			<textarea
				class="form-control"
				v-model="newMessage.text"
				placeholder="Leave your message!"
				rows="3"
			></textarea>
		</div>
	</form>
</template>

<script>
	export default {
		name: "HelloWorld",
		data() {
			return {
				newMessage: {
					title: "",
					text: "",
					timestamp: null
				}
			};
		}
	};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
	font-weight: normal;
}
ul {
	list-style-type: none;
	padding: 0;
}
li {
	display: inline-block;
	margin: 0 10px;
}
a {
	color: #42b983;
}
</style>

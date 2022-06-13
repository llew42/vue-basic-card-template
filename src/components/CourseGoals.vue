<template>
	<ul>
		<li v-for="goal in goals" :key="goal">
			<slot :goals="goal"></slot>
		</li>
	</ul>
</template>

<script>
	export default {
		data() {
			return {
				goals: ['Finish course', 'Learn Vue']
			}
		}
	};
</script>
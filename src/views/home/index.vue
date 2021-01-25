<!--  -->
<template>
	<div @click="addCount">{{count}}</div>
</template>

<script lang='ts'>
	import { ref, Ref } from "vue";
	export default {
		setup() {
			const count: Ref = ref(0);
			const addCount = (): void => {
				count.value += 1;
			};
			return { count, addCount };
		},
	};
</script>

<style lang='scss' scoped>
</style>

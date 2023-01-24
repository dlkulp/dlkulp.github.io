<script setup>
import {ref, onMounted} from "vue";
const props = defineProps({
	color: String
});
const header = ref(null);

onMounted(() => header.value.style.backgroundColor = `#${props.color}`);
</script>
<template>
	<section>
		<header ref="header">
			<i>
				<slot name="icon"></slot>
			</i>
			<h2>
				<slot name="title"></slot>
			</h2>
		</header>
		<slot></slot>
	</section>
</template>
<style scoped>
header {
	position: absolute;
	left: -2rem;
	width: calc(100% + 2rem);
	display: grid;
	place-items: center;
	align-items: center;
	place-content: center;
}

i {
	display: flex;
	place-items: center;
	place-content: center;
	width: 32px;
	height: 32px;
	color: var(--color-text);
}

h2 {
	padding-left: 5px;
}

@media (min-width: 1024px) {
	header {
		display: unset;
	}
	i {
		top: calc(50% - 25px);
		left: 25px;
		position: absolute;
		border-radius: 8px;
		width: 50px;
		height: 50px;
	}

	h2 {
		margin-left: 1rem;
		left: 50px;
		min-width: 50%;
	}
}
</style>
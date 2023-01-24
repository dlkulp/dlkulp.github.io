<script setup>
import Overview from "./components/Overview.vue";
import PageSection from "./components/PageSection.vue";
import HomeIcon from "./components/icons/IconHome.vue";
import AccountIcon from "./components/icons/IconAccount.vue";
import MusicIcon from "./components/icons/IconMusic.vue";
import GameIcon from "./components/icons/IconGame.vue";
import ChurchIcon from "./components/icons/IconChurch.vue";
</script>

<template>
	<Overview />
	<PageSection color="467545">
		<template #icon><GameIcon /></template>
		<template #title>Games</template>
		<div class="content">
			<p>Over the years I have competed in a few 24-hour programming competitions. Most of these project continued being worked on after the intial 24-hour period to add some remaining features and fix bugs.</p>
			<ul>
				<li><a href="https://gl0vgames.github.io/SneakySnake/" target="_blank">Sneaky Snake</a>: Isometric snake. Don't let the blocks see you (or your tail) as you sneak around procedurally generated levels.</li>
				<li><a href="https://gl0vgames.github.io/McClaneSim/" target="_blank">McClane Sim</a>: Die Hard's John McClane must navigate a procedurally generated building, finding weapons and other items to assist him in freeing the hostages from the terrorists while trying to stay alive. It's also a text adventure.</li>
				<li><a href="https://gl0vgames.github.io/S6/" target="_blank">S6</a>: Receive a description of your target, sneak around guards, and sling you slightly sulferous smelling smoke when you find the matching target.</li>
				<li><a href="https://fauzikliman.com/GameOfLife-3.0/" target="_blank">Game of Life 3.0</a>: Sequel to the unreleased GoL 2.0, this version uses a procedurally generated map with different values for different types of tiles.</li>
			</ul>
		</div>
	</PageSection>
	<!-- <PageSection color="678DBC">
		<template #icon><MusicIcon /></template>
		<template #title>Music</template>
		List of scores
	</PageSection> -->
	<!-- <PageSection color="88665D">
		<template #icon><ChurchIcon /></template>
		<template #title>Ministry</template>
		Stuff about minstry
	</PageSection> -->
</template>

<style scoped>
.content {
	margin-top: 4.5rem;
	display: grid;
	place-items: center;
	align-items: center;
	place-content: center;
}

@media (min-width: 1024px) {
	.content {
		margin-top: 2.5rem;
	}
}
</style>
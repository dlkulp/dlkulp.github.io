<script setup>
import DamianKulp from "../components/DamianKulp.vue";
import OverviewItem from "./OverviewItem.vue";
import MusicIcon from "./icons/IconMusic.vue";
import AccountIcon from "./icons/IconAccount.vue";
import ChurchIcon from "./icons/IconChurch.vue";
import GameIcon from "./icons/IconGame.vue";
</script>

<template>
	<section class="overview">
		<div class="center">
			<header>
				<img alt="Damian Kulp Headshot" class="logo" src="../assets/headshot.jpg" width="125" height="125" />
				<div class="wrapper">
					<DamianKulp />
				</div>
			</header>
			<article id="content">
				<OverviewItem>
					<template #icon>
						<AccountIcon />
					</template>
					<template #heading>About</template>
					I'm a seminarian at <a href="https://stots.edu" target="_blank" rel="noopener">St. Tikhon's Orthodox Theological Seminary</a>. 
					In my free time I like to teach kids music, transcribe music into English, make little browser games, and raise my son (and another on the way) with my beautiful wife Lilly.
				</OverviewItem>

				<OverviewItem>
					<template #icon>
						<MusicIcon />
					</template>
					<template #heading>Music</template>
					I was an assistant director for the Heart of the Valley Children's Choir for about 6 years and now that I'm at St. Tikhon's, I'm an assistant director in the music school, working with middle and high school students.
					I also transcribe Orthodox music into English, and I have a handful of original compositions.
					Finally, I'm working on a music aggregation project which will specialize in storing church music.
				</OverviewItem>

				<OverviewItem>
					<template #icon>
						<GameIcon />
					</template>
					<template #heading>Games</template>
					Since high school, I have enjoyed writing little browser games for competitions and for fun, using Javascript and Typescript.
				</OverviewItem>

				<!-- <OverviewItem>
					<template #icon>
						<ChurchIcon />
					</template>
					<template #heading>Ministry</template>
					As a seminarian, I will be working with St. Patrick mission in Newport, OR summer of 2023 for my internship.
				</OverviewItem> -->
			</article>
		</div>
	</section>
</template>

<style>
.overview {
	margin-top: 2rem;
	margin-bottom: 2rem;
	display: grid;
}
.overview .center {
	max-width: 1280px;
	height: 100%;
	margin: 0 auto;
	padding: 2rem;
	display: inline-grid;
	place-items: center;
	grid-template-columns: auto;
}

.overview header {
	line-height: 1.5;
}

.overview .logo {
	display: block;
	margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
	.overview header {
    	display: flex;
    	place-items: center;
    	padding-right: calc(var(--section-gap) / 2);
  	}

	.overview .logo {
		margin: 0 2rem 0 0;
	}

	.overview header .wrapper {
		display: flex;
		place-items: flex-start;
		flex-wrap: wrap;
	}

	.overview .center {
		grid-template-columns: auto auto;
	}
}
</style>
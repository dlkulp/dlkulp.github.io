<script setup>
import DamianKulp from "../components/DamianKulp.vue";
import OverviewItem from "./OverviewItem.vue";
//import HomeIcon from "./icons/IconHome.vue";
import MusicIcon from "./icons/IconMusic.vue";
import AccountIcon from "./icons/IconAccount.vue";
import ChurchIcon from "./icons/IconChurch.vue";
import GameIcon from "./icons/IconGame.vue";
</script>

<template>
	<header>
		<img alt="Damian Kulp Headshot" class="logo" src="../assets/headshot.jpg" width="125" height="125" />
		<div class="wrapper">
			<DamianKulp />
		</div>
	</header>
	<section id="overview">
		<OverviewItem>
			<template #icon>
				<AccountIcon />
			</template>
			<template #heading>About</template>
			I'm a seminarian at <a href="https://stots.edu" target="_blank" rel="noopener">St. Tikhon's Orthodox Theological Seminary</a>. 
			In my free time I like to transcribe music, make little browser games, and raise my son (and another on the way) with my beautiful wife Lilly.
		</OverviewItem>

		<OverviewItem>
			<template #icon>
				<MusicIcon />
			</template>
			<template #heading>Music</template>
			I mostly transcribe Orthodox music into English these days, though I have a handful of original compositions.
		</OverviewItem>

		<OverviewItem>
			<template #icon>
				<GameIcon />
			</template>
			<template #heading>Games</template>
			Since high school, I have enjoyed writing little browser games for competitions and for fun using Javascript and Typescript.
		</OverviewItem>

		<OverviewItem>
			<template #icon>
				<ChurchIcon />
			</template>
			<template #heading>Ministry</template>
			As a seminarian, I will be working with St. Patrick mission in Newport, OR summer of 2023 for my internship.
		</OverviewItem>
	</section>
</template>

<style scoped>
#overview {
	height: 80%;
}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
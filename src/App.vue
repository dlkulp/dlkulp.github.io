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
	<PageSection color="19a7b9">
		<template #icon><MusicIcon /></template>
		<template #title>Music</template>
		<div class="content">
			<div>
				<p>I enjoy finding recordings of Orthodox music which only exist in other languages, and transcribing them to modern English scores for liturgical use.</p>
				<p>None of these scores are original works though their transcription and translation into English is new. The general aim was to keep the melody as accurate to the original as possible while balancing natural English phrasing.</p>
			</div>
			<div class="grid">
				<article>
					<h3>Georgian</h3>
					<ul>
						<li><a target="_blank" href="/scores/Georgian/Full Dismissal - split.pdf">Dismissal</a></li>
						<li><a target="_blank" href="/scores/Georgian/Many Years.pdf">Many Years</a></li>
						<li><a target="_blank" href="/scores/Georgian/Memory Eternal.pdf">Memory Eternal</a></li>
						<li><a target="_blank" href="/scores/Georgian/Ton Despotin.pdf">Ton Despotin</a></li>
						<li><a target="_blank" href="/scores/Georgian/Georgian Paschal Troparion.pdf">Paschal Troparion (Transliterated only)</a></li>
						<li><a target="_blank" href="/scores/Georgian/Alleluia.pdf">Alleluia</a></li>
					</ul>
				</article>
				<article>
					<h3>Early Slavic Polyphony</h3>
					<ul>
						<li><a target="_blank" href="/scores/Slavic Polyphony/Great Litany.pdf">Great Litany (harmonized)</a></li>
						<li><a target="_blank" href="/scores/Slavic Polyphony/Let Our Mouths be Filled.pdf">Let Our Mouths Be Filled</a></li>
					</ul>
				</article>
				<article>
					<h3>Strochnoi</h3>
					<ul>
						<li><a target="_blank" href="/scores/Strochnoi/Great Litany.pdf">Great Litany</a></li>
						<li><a target="_blank" href="/scores/Strochnoi/O Come Let Us Worship.pdf">Come Let Us Worship</a></li>
						<li><a target="_blank" href="/scores/Strochnoi/Trisagion.pdf">Trisagion</a></li>
						<li><a target="_blank" href="/scores/Strochnoi/Our Father.pdf">Our Father</a></li>
					</ul>
				</article>
				<article>
					<h3>Znamenny</h3>
					<ul>
						<li><a target="_blank" href="/scores/Znamenny/Great Litany.pdf">Great Litany</a></li>
						<li><a target="_blank" href="/scores/Znamenny/First Antiphon.pdf">First Antiphon</a></li>
						<li><a target="_blank" href="/scores/Znamenny/Second Typical Antiphon.pdf">Second Antiphon</a></li>
						<!-- <li><a target="_blank" href="/scores/Znamenny/">God is with US</a></li> -->
					</ul>
				</article>
				<article>
					<h3>Misc</h3>
					<ul>
						<li><a target="_blank" href="/scores/Misc/Only Begotten Son - satb.pdf">Only Begotten Son - SATB</a></li>
					</ul>
				</article>
			</div>
			<div class="japanese">
				<h3>日本語 - Japanese</h3>
				<p>この音楽は英語とスラヴ語から転写されています。</p>
				<p>単語やフレーズを自然に保つように努めました。</p>
				<br />
				<div class="grid">
					<article>
						<h3>聖体礼儀</h3>
						<ul>
							<li><a target="_blank" href="/scores/日本語/連禱 - ストロクノイ.pdf">連禱のストロクノイ</a></li>
							<li><a target="_blank" href="/scores/日本語/日本の大主教聖ニコライのトロパリ.pdf">日本の大主教聖ニコライのトロパリ</a></li>
							<li><a target="_blank" href="/scores/日本語/聖なる神のビザンチンの三の調.pdf">聖なる神のビザンチンの三の調</a></li>
							<li><a target="_blank" href="/scores/日本語/ヘルビムの歌 - 4 alleluia.pdf">ヘルビムの歌</a></li>
							<li><a target="_blank" href="/scores/日本語/したしみのささげもの.pdf">したしみのささげもの</a></li>
							<li><a target="_blank" href="/scores/日本語/天にいますの四旬節の旋.pdf">天にいますの四旬節の旋</a></li>
							<li><a target="_blank" href="/scores/日本語/ハリストスの聖体を受けのアラスカのメロディ.pdf">ハリストスの聖体を受けのアラスカのメロディ</a></li>
							<li><a target="_blank" href="/scores/日本語/ハリストスの聖体を領け.pdf">ハリストスの聖体を領け</a></li>
							<li><a target="_blank" href="/scores/日本語/ハリストスの聖体を領けの一部.pdf">ハリストスの聖体を領けの一部</a></li>
							<li><a target="_blank" href="/scores/日本語/ハリストスの聖体を領けの四部.pdf">ハリストスの聖体を領けの四部</a></li>
							<li><a target="_blank" href="/scores/日本語/万寿詞.pdf">万寿詞</a></li>
						</ul>
					</article>
					<article>
						<h3>徹夜祷</h3>
						<ul>
							<li><a target="_blank" href="/scores/日本語/穏やかなる光.pdf">穏やかなる光</a></li><!--O Gladsome Light w/ transliteration-->
						</ul>
						<br />
						<h3>復活祭</h3>
						<ul>
							<li><a target="_blank" href="/scores/日本語/ハリストス死よりふくかつし.pdf">ハリストス死よりふくかつし</a></li><!--Paschal troparion w/ transliteration-->
						</ul>
					</article>
				</div>
			</div>
		</div>
	</PageSection>
	<PageSection color="DE3C4B">
		<template #icon><GameIcon /></template>
		<template #title>Games</template>
		<div class="content">
			<p>Over the years I have competed in a few 24-hour programming competitions. Most of these projects continued being worked on after the intial 24-hour period to add some remaining features and fix bugs. Enjoy!</p>
			<article>
				<h3>College</h3>
				<ul>
					<li><a href="https://gl0vgames.github.io/SneakySnake/" target="_blank">Sneaky Snake</a>: Isometric snake. Don't let the blocks see you (or your tail) as you sneak around procedurally generated levels.</li>
					<li><a href="https://gl0vgames.github.io/McClaneSim/" target="_blank">McClane Sim</a>: Die Hard's John McClane must navigate a procedurally generated building, finding weapons and other items to assist him in freeing the hostages from the terrorists while trying to stay alive. It's also a text adventure.</li>
					<li><a href="https://gl0vgames.github.io/S6/" target="_blank">S6</a>: Receive a description of your target, sneak around guards, and sling you slightly sulferous smelling smoke when you find the matching target.</li>
					<li><a href="https://fauzikliman.com/GameOfLife-3.0/" target="_blank">Game of Life 3.0</a>: Sequel to the unreleased GoL 2.0, this version uses a procedurally generated map with different values for different types of tiles.</li>
				</ul>
			</article>
			<article>
				<h3>High School</h3>
				<ul>
					<li><a href="https://tms.ogpc.info/Games/Details/717d0268-8e1a-4c10-8874-98284daec59c" target="_blank">Concepta</a>: A flying game. Help the idea of revolution spread through a population before battling the final boss in the town center.</li>
					<li><a href="https://tms.ogpc.info/Games/Details/3b2e1f39-c91c-45f9-9cdf-8d4a1ee7e11b" target="_blank">Zoning Wars</a>: A two person card game which encourages creating proper city zones.</li>
				</ul>
			</article>
		</div>
	</PageSection>
	<!-- <PageSection color="88665D">
		<template #icon><ChurchIcon /></template>
		<template #title>Ministry</template>
		Stuff about minstry
	</PageSection> -->
	<footer>
		<p>
			Website design and content:<br />© Damian Kulp {{new Date().getFullYear()}}
		</p>
	</footer>
</template>

<style scoped>
.content {
	margin-top: 5.5rem;
	display: inline-grid;
	grid-template-columns: auto;
	column-gap: 10px;
	row-gap: 20px;
}

.japanese {
	writing-mode: vertical-rl;
	text-orientation: upright;
}

.grid {
	display: inline-grid;
	grid-template-columns: auto auto;
	place-content: left;
	row-gap: 10px;
}

.grid article {
	width: 100%;
}

footer {
	width: 100%;
	display: grid;
	border-top: 2px solid var(--color-border);
}

footer p {
	text-align: center;
}

@media (min-width: 1024px) {
	.content {
		margin-top: 3.5rem;
		grid-template-columns: 25% 37.5% 37.5%;
	}
}
</style>
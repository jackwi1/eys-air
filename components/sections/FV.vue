<template>
	<div class="flex mt-[14.4vw] md:mt-[72px] w-full text-smbase md:text-base bg-white relative z-50 nav-divider text-[#222222]">
		<NuxtLink @click="() => index = 0" to="/"
			class="flex-initial h-full flex justify-center items-end w-[16.9vw] md:w-[84px] pt-[1.8vw] md:pt-[7px] pr-[1.4vw] md:pr-[3px]"
			:class="index === 0 ? 'active' : ''">
			<div class="tab-content pt-[0.45vw] md:pt-[2px] pb-[3vw] md:pb-[15px] px-[0.8vw] md:px-[4px]">
				<NuxtImg src="/img/top/icon_home.webp" loading="lazy" class="w-[3.7vw] md:w-[19px] h-[3.65vw] md:h-[21px]"
					alt="Home" />
			</div>
		</NuxtLink>

		<NuxtLink @click="() => index = 1" to="/" class="flex-initial h-full flex justify-center items-end pt-[1.8vw] md:pt-[8px] w-[20.5vw] md:w-[103px]"
			:class="index === 1 ? 'active' : ''">
			<div class="tab-content pb-[1.8vw] md:pb-[8px] px-[5px]">
			<span>音楽</span>
		</div>
		</NuxtLink>

		<NuxtLink @click="() => index = 2" to="/" class="flex-initial h-full flex justify-center items-end pt-[1.8vw] md:pt-[8px] w-[23vw] md:w-[116px]"
			:class="index === 2 ? 'active' : ''">
			<div class="tab-content pb-[1.8vw] md:pb-[8px] px-[5px]">
			<span>ワイン</span>
		</div>
		</NuxtLink>

		<NuxtLink @click="() => index = 3" to="/" class="flex-initial h-full flex justify-center items-end pt-[1.8vw] md:pt-[8px] w-[20.6vw] md:w-[102.5px]"
			:class="index === 3 ? 'active' : ''">
			<div class="tab-content pb-[1.8vw] md:pb-[8px] px-[5px]">
			<span>茶道</span>
		</div>
		</NuxtLink>

		<NuxtLink @click="() => index = 4" to="/" class="flex-1 h-full flex justify-center items-end pt-[1.8vw] md:pt-[8px] pl-[2vw] md:pl-[10px] "
			:class="index === 4 ? 'active' : ''">
			<div class="tab-content pb-[1.8vw] md:pb-[8px] px-[5px]">
			<span>陶芸</span>
		</div>
		</NuxtLink>
	</div>
	<div class="relative  pb-[0.8vw] md:pb-[38px]">
		<NuxtImg src="/img/top/FV.webp" class="w-full h-[160.2vw] md:h-[802px] absolute top-[-0.38vw] md:top-[-1.9px] left-0" alt="FV_bg" />

		<div class="relative z-10 flex flex-col items-center pt-[5vw] md:pt-[30px]">
			<div class="flex justify-center items-center">
				<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[3vw] md:w-[15px] h-[4vw] md:h-[20px]"
					alt="backslash" />
				<h3 class="text-[4vw] md:text-[20px] text-center mx-[2vw] md:mx-[10px] font-semibold tracking-normal">
					驚きのクレイジー特典を、無料プレゼント！
				</h3>
				<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[3vw] md:w-[15px] h-[4vw] md:h-[20px]" alt="slash" />
			</div>
			<h2 class="text-[6.4vw] md:text-[32px] pt-[1vw] md:pt-[5px] my-[2vw] md:my-[6px] font-bold tracking-wider">EYSのオンラインアカデミー</h2>
		</div>

		<div class="flex justify-evenly mt-[2.7vw] md:mt-[17px] mx-[7vw] md:mx-[35px]">
			<div class="relative">
				<MoleculesFVIteam tit="音楽" startColor="#7799FF" endColor="#77DDFF" img="/img/top/music.webp" txt="楽器"
					class="relative z-10" />
				<NuxtImg src="/img/top/music-ring.webp" loading="lazy"
					class="w-[18.7vw] md:w-[93px] h-[18.7vw] md:h-[93px] absolute left-[-6.8vw] md:left-[-33px] top-[0.3vw] md:top-[3px]"
					alt="music-ring" />
			</div>
			<div class="relative">
				<MoleculesFVIteam tit="ワイン" startColor="#EE88BB" endColor="#FFCC99" img="/img/top/wine.webp" txt="ワイングラス"
					class="relative z-10" customTitlePadding="px-[3vw] md:px-[14.5px]" customDecPadding="px-[3.5vw] md:px-[16.5px]" />
				<NuxtImg src="/img/top/wine-ring.webp" loading="lazy"
					class="w-[13.1vw] md:w-[65px] h-[13.1vw] md:h-[65px] absolute right-[-6.5vw] md:right-[-32.5px] top-[10vw] md:top-[50.5px]"
					alt="wine-ring" />
			</div>
		</div>
		<div class="flex justify-between mt-[-4.8vw] md:mt-[-25px] px-[3vw] md:px-[13px]">
			<div class="relative">
				<MoleculesFVIteam tit="茶道" startColor="#99DD77" endColor="#EEEE55" img="/img/top/tea.webp" txt="茶釜・畳"
					class="relative z-10" />
				<NuxtImg src="/img/top/tea-ring.webp" loading="lazy"
					class="w-[11.25vw] md:w-[55px] h-[11.25vw] md:h-[55px] absolute right-[-5.3vw] md:right-[-27px] top-[8vw] md:top-[41px]"
					alt="tea-ring" />
			</div>
			<div class="relative">
				<MoleculesFVIteam tit="陶芸" startColor="#BBAA88" endColor="#EEDD55" img="/img/top/pottery.webp" txt="焼き窯"
					class="relative z-10" />
				<NuxtImg src="/img/top/pottery-ring.webp" loading="lazy"
					class="w-[8.8vw] md:w-[44px] h-[8.8vw] md:h-[44px] absolute right-[-0.3vw] md:right-[1.5px] bottom-[12.78vw] md:bottom-[65px]"
					alt="pottery-ring" />
			</div>
		</div>
		<div class="flex justify-center">
			<NuxtImg src="/img/top/mockup.webp" loading="lazy" width="100%" height="auto"
				class="w-[75.5vw] md:w-[376px] h-[50.2vw] md:h-[251px] top-[3.49vw] md:top-[16.8px] relative z-10" alt="mockup" />
		</div>
	</div>
</template>

<script lang="ts" setup>
const index = useState('index', () => 0);
</script>

<style scoped>
.nav-divider > * {
	position: relative;
}

.tab-content {
	border-bottom: 3px solid transparent;
	box-sizing: border-box;
}

.active .tab-content {
	border-bottom-color: #000000;
}

.nav-divider > :not(:first-child)::before {
	content: "";
	position: absolute;
	left: 0;
	top: 30%;
	bottom: 30%;
	width: 1px;
	background-color: #DDDDDD;
}

</style>
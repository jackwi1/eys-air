<template>
	<div class="relative overflow-x-clip">
		<div class="flex flex-col justify-center items-center mt-[12.5vw] md:mt-[65px] relative">
			<NuxtImg src="/img/event/event-logo.webp" loading="lazy" width="100%" height="auto"
				class="w-[26.8vw] md:w-[130px] h-[10.7vw] md:h-[50px] mb-[4.4vw] md:mb-[20px]" alt="event-logo" />
			<div class="flex justify-center items-end">
				<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]"
					alt="backslash" />
				<h3 class="text-[4.5vw] md:text-[23px] text-center mx-[2.8vw] md:mx-[13px] font-bold leading-snug">
					スクールで恋して結婚へ...<br>EYSが提案する新しい出会い
				</h3>
				<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]" alt="slash" />
			</div>
			<NuxtImg src="/img/event/event-ring.webp" loading="lazy"
				class="absolute w-[32vw] md:w-[160px] h-[32vw] md:h-[160px] right-[-8.5vw] md:right-[-44px] top-[-8.4vw] md:top-[-45px]"
				alt="event-ring" />

			<NuxtImg src="/img/event/event-bg.webp" loading="lazy" class="w-full h-[53.4vw] md:h-[268px] mt-[4vw] md:mt-[20px]"
				alt="evnet-bg" />

			<div class="px-[3vw] md:px-[15px] pt-[4.2vw] md:pt-[20px] pb-[3vw] md:pb-[15px] w-[100%]">
				<AtomsHeadTitle3 text="趣味を通じて自然に仲良くなれる、<br>様々なイベントを開催しています！" startColor="#55CCAA" endColor="#88DD77"
					class="relative top-[-12vw] md:top-[-60px]" customPadding2="px-[6.6vw] md:px-[33px]" />
				<div class="flex flex-wrap justify-between gap-y-[2.7vw] md:gap-y-[12px] relative top-[-7vw] md:top-[-35px]">
					<MoleculesEVNTRCard img="/img/event/event1.webp" tit="料理合コン" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/event/event2.webp" tit="ゴルフ合コン" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/event/event3.webp" tit="ワイン合コン" class="w-[32%]" />
				</div>
			</div>

			<div class="relative top-[-4.7vw] md:top-[-24px] flex justify-center w-[53.34%] mx-auto">
				<AtomsComButton btnText="スク婚ページへ" linkUrl="/" imgUrl="/img/arrow.webp" />
			</div>
		</div>

	</div>
</template>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY > 1400) {
		showElement.value = true
	} else {
		showElement.value = false
	}
}

onMounted(() => {
	window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
	window.removeEventListener('scroll', handleScroll)
})
</script> -->
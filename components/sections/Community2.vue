<template>
	<div class="relative overflow-x-clip mb-[9.5vw] md:mb-[46.5px]">
		<div class="flex flex-col justify-center items-center mt-[7.5vw] md:mt-[38px] relative">
			<NuxtImg src="/img/community2/v2-logo.webp" loading="lazy"
				class="w-[65vw] md:w-[325px] h-[13vw] md:h-[65px] mb-[3.5vw] md:mb-[16px]" alt="v2-logo" />
			<div class="flex justify-center items-end">
				<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]"
					alt="backslash" />
				<h3 class="text-[4.3vw] leading-[6vw] md:text-[21.5px] md:leading-[30px] text-center mx-[6.5vw] md:mx-[34.5px] font-bold tracking-loose">
					2nd Community アプリで、<br>更に出会いと繋がりが拡大！
				</h3>
				<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]" alt="slash" />
			</div>
			<NuxtImg src="/img/community2/ring.webp" loading="lazy" width="100%" height="auto"
				class="absolute w-[32vw] md:w-[160px] h-[32vw] md:h-[160px] left-[-18vw] md:left-[-100px] top-[-12vw] md:top-[45px]"
				alt="v2-ring" />

			<NuxtImg src="/img/community2/v2-bg.webp" loading="lazy"
				class="w-full mt-[4.1vw] md:mt-[22px] h-[53.6vw] md:h-[268px]" alt="v2-bg" />

			<div class="p-[3vw] md:p-[15px] w-[100%]">
				<AtomsTitle2 text="趣味やライフイベントに合わせた、<br>多彩なコミュニティをご用意しています！" startColor="#55CCAA" endColor="#88DD77"
					class="relative top-[-11vw] md:top-[-57px]" />
				<div class="flex flex-wrap justify-between gap-y-[2.4vw] md:gap-y-[12px] relative top-[-5.8vw] md:top-[-29px]">
					<MoleculesComCard img="/img/community2/set1.webp" class="w-[48.3%]" />
					<MoleculesComCard img="/img/community2/set2.webp" class="w-[48.3%] relative z-10" />
					<NuxtImg src="/img/event/event-ring.webp" loading="lazy" width="100%" height="auto"
						class="absolute w-[19.1vw] md:w-[95px] h-[19.1vw] md:h-[95px] right-[-12.5vw] md:right-[-61.5px] bottom-[-9.3vw] md:bottom-[-46.5px]"
						alt="event-ring" />
				</div>
			</div>

			<div class="p-[1.4vw] md:p-[7px] mt-[5vw] md:mt-[25px]">
				<AtomsTitle2 text="例えば、<br>こんなコミュニティ！" startColor="#55CCAA" endColor="#88DD77"
					class="relative top-[-10vw] md:top-[-50px]" custom2="px-[5.3vw] md:px-[26.5px]" />
			</div>
			<div class="w-full relative bottom-[6vw] md:bottom-[30px] top-[-6.3vw] md:top-[-32.5px]">
				<Swiper :slides-per-view="1.5" :effect="'creative'" :creative-effect="{
					prev: {
						translate: ['-20%', 0, 0],
					},
					next: {
						translate: ['100%', 0, 0],
					},
				}" :initial-slide="1" :centered-slides="true">
					<SwiperSlide>
						<NuxtImg src="/img/community2/slider1.webp" loading="lazy"
							class="w-[66vw] md:w-[330px] h-[123vw] md:h-[615px]" alt="com-v2-slider1" />
					</SwiperSlide>

					<SwiperSlide>
						<NuxtImg src="/img/community2/slider1.webp" loading="lazy"
							class="w-[66vw] md:w-[330px] h-[123vw] md:h-[613px]" alt="com-v2-slider2" />
					</SwiperSlide>

					<SwiperSlide>
						<NuxtImg src="/img/community2/slider1.webp" loading="lazy"
							class="w-[66vw] md:w-[330px] h-[123vw] md:h-[615px]" alt="com-v2-slider3" />
					</SwiperSlide>
				</Swiper>
			</div>

			<div class="flex justify-center w-[53.4%] mx-auto relative top-[-1.1vw] md:top-[-6.5px]">
				<AtomsComButton btnText="コミュニティ一覧" linkUrl="/" imgUrl="/img/arrow.webp" />
			</div>
		</div>
	</div>
</template>

<style scoped>
.swiper-slide {
	transform: scale(0.8);
}

.swiper-slide-active {
	transform: scale(1);
}
</style>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY > 1800) {
		showElement.value = true
	} else {
		showElement.value = false
	}
}

onMounted(() => {
	window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
	window.removeEventListener('scroll', handleScrroll)
})
</script> -->
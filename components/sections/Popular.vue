<template>
	<div class="relative overflow-x-clip mt-[5.5vw] md:mt-[15px]">
		<AtomsSectionTitle text="人気のジャンル/コース" class="relative z-10 pt-[13vw] md:pt-[80px] pb-[10vw] md:pb-[50px]" />
		<NuxtImg src="/img/pop/pop-ring.webp" loading="lazy"
			class="absolute w-[30vw] md:w-[153px] h-[32vw] md:h-[159px] left-[-13vw] md:left-[-67px] top-[21vw] md:top-[116px]"
			alt="pop-ring" />
		<NuxtImg src="/img/pop/pop-bg.webp" loading="lazy"
			class="absolute w-[98vw] md:w-[490px] h-[80vw] md:h-[400px] right-[-21vw] md:right-[-105px] top-[-17.5vw] md:top-[-75px]"
			alt="popular" />
		<div class="swiper">
			<Swiper class="pop-swiper" :slides-per-view="1.32" :effect="'creative'" :creative-effect="{
				prev: {
					translate: ['-100%', 0, 0],
				},
				next: {
					translate: ['100%', 0, 0],
				},
			}">
				<SwiperSlide>
					<AtomsCard class="w-[62.7vw] md:w-[330px] h-[181.35vw] md:h-[680px] rounded-md">
						<OrganismsPopCard text="音楽" startColor="#7799FF" endColor="#77DDFF" imgSrc="/img/pop/music.webp"
							benefitTxt="サックスプレゼント" benefitImg="/img/pop/music-benefit.webp" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[64vw] md:w-[330px] h-[181.35vw] md:h-[680px] rounded-md">
						<OrganismsPopCard text="ワイン" startColor="#EE88BB" endColor="#FFCC99" imgSrc="/img/pop/wine.webp"
							benefitTxt="ワイングラスプレゼント" benefitImg="/img/pop/wine-benefit.webp" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[66vw] md:w-[330px] h-[181.35vw] md:h-[680px] rounded-md">
						<OrganismsPopCard text="茶道" startColor="#99DD77" endColor="#EEEE55" imgSrc="/img/pop/music.webp"
							benefitTxt="茶釜・畳プレゼント" benefitImg="/img/pop/tea-benefit.webp" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[66vw] md:w-[330px] h-[181.35vw] md:h-[680px] rounded-md">
						<OrganismsPopCard text="陶芸" startColor="#BBAA88" endColor="#EEDD55" imgSrc="/img/pop/wine.webp"
							benefitTxt="焼き窯プレゼント" benefitImg="/img/pop/pottery-benefit.webp" />
					</AtomsCard>
				</SwiperSlide>
			</Swiper>
		</div>

		<OrganismsEYSWatch/>
	</div>
</template>

<style scoped>
.pop-swiper {
	position: relative;
	padding-left: 5.4vw;
}

@media (min-width: 500px) {
	.pop-swiper {
		padding-left: 27px;
	}
}
</style>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY >= 100) {
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
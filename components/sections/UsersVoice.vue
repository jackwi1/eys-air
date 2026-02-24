<template>
	<div>
		<NuxtImg src="/img/voice/voice-tit.webp" loading="lazy" class="w-[70vw] md:w-[350px] h-[23vw] md:h-[115px]  mx-auto"
			alt="user's voice" />

		<div class="relative">
			<Swiper ref="swiperRef" class="mt-[6.7vw] md:mt-[23px] md:mb-[7px] voice-swiper" :slides-per-view="1.6" :effect="'creative'" :creative-effect="{
				prev: {
					translate: ['-100%', 0, 0],
				},
				next: {
					translate: ['100%', 0, 0],
				},
			}" :initial-slide="1" :centered-slides="true">
				<SwiperSlide>
					<MoleculesVoice socialImg="/img/voice/instagram.webp" userImg="/img/voice/user2.webp"
						mainImg="/img/voice/bg2.webp" />
				</SwiperSlide>
				<SwiperSlide>
					<MoleculesVoice socialImg="/img/voice/facebook.webp" userImg="/img/voice/user2.webp"
						mainImg="/img/voice/bg2.webp" />
				</SwiperSlide>
				<SwiperSlide>
					<MoleculesVoice socialImg="/img/voice/instagram.webp" userImg="/img/voice/user2.webp"
						mainImg="/img/voice/bg2.webp" />
				</SwiperSlide>
			</Swiper>

			<button @click="slidePrev" class="absolute left-[0vw] top-[2.7vw] md:top-[26px] z-20 cursor-pointer transition-opacity">
				<NuxtImg src="/img/voice/arrow-left.webp" loading="lazy" class="w-[13vw] md:w-[67px] h-[13vw] md:h-[67px]" alt="Previous" />
			</button>

			<button @click="slideNext" class="absolute right-[0vw] top-[2.7vw] md:top-[26px] z-20 cursor-pointer transition-opacity">
				<NuxtImg src="/img/voice/arrow-right.webp" loading="lazy" class="w-[13vw] md:w-[67px] h-[13vw] md:h-[67px]" alt="Next" />
			</button>
		</div>
	</div>
</template>

<script setup>
import { ref } from 'vue'

const swiperRef = ref(null)

const slidePrev = () => {
	if (swiperRef.value && swiperRef.value.$el.swiper) {
		swiperRef.value.$el.swiper.slidePrev()
	}
}

const slideNext = () => {
	if (swiperRef.value && swiperRef.value.$el.swiper) {
		swiperRef.value.$el.swiper.slideNext()
	}
}
</script>

<style scoped>
.swiper {
	padding-bottom: 24px;
	position: relative;
	z-index: 10;
}

.swiper-slide {
	position: relative;
	top: 60px;
	opacity: 0.5;
	transition: transform 0.3s ease;
}

.swiper-slide-active {
	transform: scaleX(1.1);
	top: 0;
	opacity: 1;
	z-index: 10;
}
</style>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY > 600) {
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
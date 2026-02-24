<template>
	<div>
		<div class="relative overflow-x-clip py-[2vw] md:py-[15px] mb-[0.8vw] md:mb-[0.5px]">
			<NuxtImg src="/img/reason/v1/bg.webp" loading="lazy" class="w-full h-[100vw] md:h-[500px]" alt="reason-v1-bg" />
			<p
				class="text-center absolute z-10 left-0 top-[34.5%] md:top-[36%] text-[4.28vw] md:text-[21px] w-full leading-[6vw] md:leading-[28px] font-bold">
				オンラインでも<br>リアルのレッスンと変わらない<br>「仕掛け」があります！
			</p>
			<div class="absolute w-full top-[60.8%]">
				<MoleculesReasonTitle number="01" text="全ジャンル<br>クレイジー特典プレゼント！" />
			</div>
		</div>
		<div class="flex flex-row flex-wrap overflow-hidden">
			<div v-for="(feature, index) in features" :key="index" class="w-[50%]">
				<OrganismsReasonFeature :index="index" :titTxt="feature.titTxt" :startColor="feature.startColor"
					:endColor="feature.endColor" :subTxt="feature.subTxt" :text="feature.text" :imgUrl="feature.imgUrl"
					:linkUrl="feature.linkUrl" 
					:customTitlePadding="index === 1 ? 'px-[3vw] md:px-[15px]' : undefined"
					:customImageSetting1="index % 2 === 0 ? 'relative h-[100.3vw] md:h-[501px] w-[48vw] md:w-[240px] left-[-2vw] md:left-[-10px] top-[-0.7vw] md:top-[-3.5px]' : undefined"
					:customImageSetting2="index % 2 !== 0 ? 'relative h-[100.3vw] md:h-[501px] w-[48vw] md:w-[240px] right-[-1.4vw] md:right-[-7px] top-[-0.7vw] md:top-[-3.5px]' : undefined"
					:customBottom="index < 2 ? 'mb-[3vw] md:mb-[17px]' : undefined"
					/>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	data() {
		return {
			features: [
				{
					titTxt: "音楽",
					startColor: "#7799FF",
					endColor: "#77DDFF",
					subTxt: "ギター・サックス・ピアノ...",
					text: "高品質な楽器を<br>無料でプレゼント！",
					imgUrl: "/img/reason/v1/feature1.webp",
					linkUrl: "/",
				},
				{
					titTxt: "ワイン",
					startColor: "#EE88BB",
					endColor: "#FFCC99",
					subTxt: "ワイングラス・高級ワイン...",
					text: "テイスティングセットを<br>無料でプレゼント！",
					imgUrl: "/img/reason/v1/feature2.webp",
					linkUrl: "/",
				},
				{
					titTxt: "茶道",
					startColor: "#99DD77",
					endColor: "#EEEE55",
					subTxt: "茶道具・畳・茶釜・和菓子...",
					text: "茶道具一式を<br>無料でプレゼント！",
					imgUrl: "/img/reason/v1/feature3.webp",
					linkUrl: "/",
				},
				{
					titTxt: "陶芸",
					startColor: "#BBAA88",
					endColor: "#EEDD55",
					subTxt: "焼き窯・ろくろ・粘土...",
					text: "陶芸完結セットを<br>無料でプレゼント！",
					imgUrl: "/img/reason/v1/feature4.webp",
					linkUrl: "/",
				}
			]
		}
	}
}
</script>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY > 500) {
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
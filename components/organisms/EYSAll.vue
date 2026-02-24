<template>
	<div class="py-[5vw] md:py-[17.5px]">
		<h4 class="text-center text-smsub md:text-sub text-[#222222] leading-[6.7vw] md:leading-[32.5px]">
			老若男女・性別・経験を問わず、<br>幅広くご支持いただいています！
		</h4>
		<div class="flex justify-center">
			<div class="border-b-2 my-[3.5vw] md:my-[20px] border-[#999999] border-solid w-[11vw] md:w-[60px]"></div>
		</div>

		<AtomsTitle text="男女比" startColor="#77DDFF" endColor="#7799FF" class="mb-[2.2vw] md:mb-[16px] mt-[1vw] md:mt-[5.3px]"  />

		<h4 class="text-center text-smsub md:text-sub text-blue leading-[6.4vw]">
			男性にも女性にも、<br>お楽しみいただいています！
		</h4>

		<NuxtImg src="/img/news/rate-chart.webp" loading="lazy"
			class="w-[81.4vw] md:w-[407px] h-[62.7vw] md:h-[315px] my-[3.6vw] md:my-[22px] mx-auto" alt="rate-chart" />

		<AtomsTitle text="年代分布" startColor="#77DDFF" endColor="#7799FF" customAgePadding="px-[6.65vw] md:px-[37px]" class="my-[2vw] md:my-[10px] top-[1vw] md:top-[3px]" />

		<h4 class="text-center text-smsub md:text-sub pt-[1vw] md:pt-[7px] text-blue leading-[6.5vw]">
			年代別・レベル別のクラス分けで、<br>安心してレッスンを受けられます！
		</h4>

		<NuxtImg src="/img/news/age-chart.webp" loading="lazy"
			class="w-[90vw] md:w-[450px] h-[66.5vw] md:h-[340px] mt-[1vw] md:mt-[5px] mb-[3.1vw] md:mb-[23.5px]" alt="age-chart" />
	</div>
</template>

<style scoped>
.rate-chart {
	width: 200px;
	height: 200px;
	border-radius: 50%;
	background-image: conic-gradient(#FF99CC 216deg, #7799FF 0);
	position: relative;
	overflow: hidden;
}
</style>
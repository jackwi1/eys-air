<template>
	<div class="flex flex-col justify-center items-center relative">
		<div class="text-white py-[1.6vw] md:py-[9.5px] pt-[2.1vw] pb-[1.7vw] transform skew-x-[-25deg]"
			:class="[customReasonFeature1 || customReasonFeature2 || 'px-[6.2vw] md:px-[35px]']"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }">
			<p class="text-[4vw] text-center md:text-[20px] leading-[6vw] md:leading-[30px] px-[2vw] md:px-[10px] transform skew-x-[25deg] font-bold"
				v-html="text">
			</p>
		</div>
		<div class="arrow absolute h-[2.8vw] md:h-[15px] w-[5vw] md:w-[25px]"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }"></div>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'startColor',
		'endColor',
		'customReasonFeature1',
		'customReasonFeature2',
	]
}
</script>

<style scoped>
.arrow {
	clip-path: polygon(50% 100%, 100% 0%, 0% 0%);
	top: 98%;
}
</style>
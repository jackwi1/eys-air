<template>
	<div class="flex flex-col justify-center items-center relative">
		<div :class="['text-white py-[2.45vw] md:py-[8px] transform skew-x-[-25deg]', customAgePadding || 'px-[8.67vw] md:px-[48px]']"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }">
			<p class="text-[3.8vw] text-center md:text-[19px] leading-[5vw] md:leading-[25px] transform skew-x-[25deg]"
				v-html="text">
			</p>
		</div>
		<div class="arrow absolute h-[2vw] md:h-[10px] w-[4vw] md:w-[20px]"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }"></div>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'startColor',
		'endColor',
		'customAgePadding'
	]
}
</script>

<style scoped>
.arrow {
	clip-path: polygon(50% 100%, 100% 0%, 0% 0%);
	top: 100%;
}
</style>
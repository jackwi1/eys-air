<template>
	<div class="flex flex-col justify-center items-center relative">
		<div :class="['text-white py-[1.9vw] md:py-[10px] transform skew-x-[-25deg]', customAgePadding || custom2 || 'px-[3.3vw] md:px-[18px]']"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }">
			<p class="text-[4vw] text-center md:text-[20px] leading-[6vw] md:leading-[30px] transform skew-x-[25deg] font-bold tracking-normal"
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
		'customAgePadding',
		'custom2',
	]
}
</script>

<style scoped>
.arrow {
	clip-path: polygon(50% 100%, 100% 0%, 0% 0%);
	top: 100%;
}
</style>
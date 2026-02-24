<template>
	<div class="flex flex-col justify-center items-center relative">
		<div class="text-white pt-[2.1vw] md:pt-[10.5px] pb-[1.7vw] md:pb-[8.5px] transform skew-x-[-25deg]"
			:class="[customPadding || customPadding2 || 'px-[2.6vw]', 'md:px-[13px]']"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }">
			<p class="text-[4vw] text-center md:text-[20px] leading-[6vw] md:leading-[30.5px] tracking-normal transform skew-x-[25deg]"
				v-html="text">
			</p>
		</div>
		<div class="arrow absolute h-[2.8vw] md:h-[14px] w-[5vw] md:w-[25px]"
			:style="{ background: `linear-gradient(45deg, ${startColor}, ${endColor})` }"></div>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'startColor',
		'endColor',
		'customPadding',
		'customPadding2',
	]
}
</script>

<style scoped>
.arrow {
	clip-path: polygon(50% 100%, 100% 0%, 0% 0%);
	top: 98%;
}
</style>
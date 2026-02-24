<template>
	<div class="flex justify-start items-center">
		<div :class="['relative text-white py-[0.6vw] md:py-[3px] transform skew-x-[-25deg]', customTitlePadding || 'px-[4.73vw] md:px-[25px]']"
			:style="{ background: `linear-gradient(to right, ${startColor}, ${endColor})` }">
			<p class="text-smbase md:text-base transform skew-x-[25deg]">{{ text }}</p>
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'startColor',
		'endColor',
		'customTitlePadding'
	]
}
</script>

<style scoped></style>
<template>
	<div class="flex justify-start items-center">
		<div :class="['relative text-white py-[2.7vw] md:py-[13.25px] transform skew-x-[-25deg]', customPadding || 'px-[4.3vw] md:px-[24.5px]']"
			:style="{ background: `linear-gradient(to right, ${startColor}, ${endColor})` }">
			<p class="text-[5.35vw] md:text-[26.75px] transform skew-x-[25deg] font-bold">{{ text }}</p>
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'startColor',
		'endColor',
		'customPadding',
	]
}
</script>

<style scoped></style>
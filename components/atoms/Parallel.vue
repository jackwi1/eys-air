<template>
	<div class="flex justify-start items-center">
		<div :class="['relative text-white py-[2.95vw] md:py-[15px] transform skew-x-[-25deg]', customPadding || 'px-[8.2vw] md:px-[43px]']"
			:style="{ background: `linear-gradient(to right, ${startColor}, ${endColor})` }">
			<p class="text-[4.8vw] md:text-[24px] transform skew-x-[25deg]">{{ text }}</p>
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
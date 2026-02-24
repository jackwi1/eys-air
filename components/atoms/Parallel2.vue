<template>
	<div class="flex justify-start items-center">
		<div class="relative text-white py-[2.95vw] md:py-[18px] transform skew-x-[-25deg] px-[8.4vw] md:px-[45px]"
			:style="{ background: `linear-gradient(to right, ${startColor}, ${endColor})` }">
			<p class="text-[8vw] font-bold italic leading-[18px] md:text-[40px] transform skew-x-[25deg]">{{ text }}</p>
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
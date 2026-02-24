<template>
	<div class="flex flex-col items-center">
		<AtomsReasonParallel :text="tit" :startColor="startColor" :endColor="endColor" :customTitlePadding="customTitlePadding" class="relative z-10" />
		<NuxtImg :src="img" loading="lazy"
			class="w-[26.7vw] md:w-[133.5px] h-[26.7vw] md:h-[133.5px] relative top-[-3.7vw] md:top-[-18.5px]" :alt="tit" />
		<div
			:class="['flex flex-col gap-0 leading-tight bg-black text-white rounded-full text-center py-[0.88vw] md:py-[1px] relative top-[-6.7vw] md:top-[-34px]', customDecPadding || 'px-[2.7vw] md:px-[13.5px]']">
			<span class="text-smbase md:text-base leading-tight tracking-normal">{{ txt }}</span>
			<span class="text-[2.6vw] md:text-[13px] leading-tight tracking-normal">プレゼント！</span>
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'tit',
		'startColor',
		'endColor',
		'img',
		'txt',
		'customTitlePadding',
		'customDecPadding'
	]
}
</script>

<style scoped></style>
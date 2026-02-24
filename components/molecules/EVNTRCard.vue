<template>
	<div class="flex flex-col justify-between items-center">
		<AtomsCard class="flex flex-col rounded-[10px]">
			<NuxtImg :src="img" loading="lazy" class="w-[29.4vw] md:w-[147px] h-[21.2vw] md:h-[107px]" alt="evntr-card" />
			<p class="text-[3vw] md:text-[15px] py-[2.6vw] md:py-[13px] tracking-tighter" v-if="tit">{{ tit }}</p>
		</AtomsCard>
	</div>
</template>

<script>
export default {
	props: [
		"img",
		"tit",
	]
}
</script>
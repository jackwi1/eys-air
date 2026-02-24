<template>
	<h4 class="text-[4.3vw] md:text-[23px] font-medium mt-[4vw] md:mt-[20px]">{{ tit }}</h4>
	<div class="flex flex-row w-full justify-start mt-[4vw] md:mt-[20px]">
		<NuxtImg :src="avatar" loading="lazy" class="w-[10vw] md:w-[50px] h-[10vw] md:h-[50px]" alt="avatar" />
		<div class="flex flex-col justify-center ml-[4vw] md:ml-[20px] text-smmini md:text-mini">
			<span class="font-extrabold font-avenir" :style="{ color: `${color}` }">EVNTR</span>
			<span>{{ school }}</span>
		</div>
	</div>
	<p class="text-[3vw] md:text-[15px] leading-[5.1vw] md:leading-[25px] tracking-[-0.2vw] md:tracking-[-1px] px-[1.3vw] md:px-[6.5px] py-[1.2vw] md:py-[6px] font-light">{{ desc }}</p>
	<div class="flex justify-start items-center w-full px-[1.3vw] md:px-[6.5px]">
		<NuxtImg src="/img/yen.webp" loading="lazy" class="w-[4vw] md:w-[20px] h-[4vw] md:h-[20px]" alt="yen" />
		<span class="ml-[2vw] md:ml-[10px] text-smbase md:text-base">{{ price }}</span>
	</div>
	<AtomsRoundButton :startColor="startColor" :endColor="endColor" :linkUrl="linkUrl" />
</template>

<script>

export default {
	props: [
		'tit',
		'avatar',
		'color',
		'school',
		'desc',
		'price',
		'startColor',
		'endColor',
		'linkUrl',
	]
}
</script>

<style scoped></style>
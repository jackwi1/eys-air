<template>
	<div class="relative z-10 mt-[2.6vw] md:mt-[13px] shadow-xl">
		<AtomsHeadTitle :text="text" startColor="#FF6E6E" endColor="#FFBCDD" class="relative top-[3vw] md:top-[15px]" :customReasonFeature1="customReasonFeature1" :customReasonFeature2="customReasonFeature2" />
		<NuxtImg :src="img" loading="lazy" class="w-full h-[50.15vw] md:h-[250px]" alt="feature-img" />
		<p class="text-center bg-white border-[2px] border-solid border-[#F6F6F6] text-[4vw] md:text-[20px] leading-[5.87vw] md:leading-[27.5px] pt-[4vw] md:pt-[25px] pb-[3.75vw] md:pb-[18.75px] rounded-[2vw] md:rounded-[10px] w-[106%] left-[-3%] relative tracking-normal shadow-xl"
			v-html="desc">
		</p>
	</div>
</template>

<script>

export default {
	props: [
		'text',
		'img',
		'desc',
		'customReasonFeature1',
		'customReasonFeature2',
	]
}
</script>
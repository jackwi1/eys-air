<template>
	<div class="relative">
		<NuxtImg :src="mainImg" loading="lazy" class="w-[94.2%] h-[63vw] md:h-[320px]" alt="pagination-main" />
		<div class="flex flex-col items-end absolute right-0 top-[87%] md:top-[86%]">
			<AtomsCard class="relative w-[94.2%] rounded-[4vw] md:rounded-[20px]">
				<div
					class="flex flex-col px-[3.6vw] md:px-[18px] pt-[4vw] md:pt-[20px] pb-[3.6vw] md:pb-[40px] pr-[34vw] md:pr-[170px] text-smsub md:text-sub rounded-[4vw] md:rounded-[20px]">
					<p class="text-[4.8vw] md:text-[21px] leading-[6.4vw] md:leading-[32px] tracking-normal">{{ text }}</p>
					<span
						class="text-[#DDDDDD] text-end font-apple text-smlarge md:text-large relative top-[1vw] md:top-[35px] left-[-2vw] md:left-[-10px]">{{
							nameEn
						}}</span>
					<span class="text-[3.6vw] md:text-[18px] mt-[-3vw] md:mt-[15px] relative z-50">{{ nameJp }}</span>
					<span class="text-smmini md:text-mini text-[#666666] font-light">{{ details }}</span>
				</div>
				<NuxtImg :src="relImg" loading="lazy"
					class="absolute right-[7.28vw] md:right-[36px] w-[28.7vw] md:w-[144px] h-[76vw] md:h-[381px] translate-y-[-50%] top-[50.5%]"
					alt="rel-img" />
			</AtomsCard>
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'mainImg',
		'relImg',
		'text',
		'nameEn',
		'nameJp',
		'details',
	]
}
</script>
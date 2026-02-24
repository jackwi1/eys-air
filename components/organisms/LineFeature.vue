<template>
	<div class="relative" :class="[index ? 'mt-[27vw] md:mt-[135px]' : '']">
		<div class="relative flex flex-col items-center justify-center z-10">
			<AtomsParallel :text="titTxt" :startColor="startColor" :endColor="endColor" :customPadding="customPadding" class="relative z-20 md:bottom-[-9px]" />
			<div class="relative flex items-center flex-col">
				<NuxtImg :src="topImg" loading="lazy" class="relative top-[-5.3vw] md:top-[-18px] w-full h-[53vw] md:h-[265px]"
					alt="top-img" />
				<div class="absolute transform translate-y-[-55%] flex flex-col items-center w-[83.62%] top-[96%] md:top-[99%]">
					<NuxtImg :src="iPadImg" loading="lazy" class="w-full h-[53.4vw] md:h-[267px]" alt="ipad-img" />
					<div class="absolute bottom-[3vw] md:bottom-[15px] w-[90%] border-[1px] border-solid border-white">
						<AtomsGotoButton :btnText="btnTxt" :linkUrl="linkUrl" />
					</div>
				</div>
			</div>
		</div>
		<div v-if="index === 0">
			<NuxtImg :src="ringImg" loading="lazy"
				class="absolute w-[32vw] md:w-[160px] h-[32vw] md:h-[160px] right-[-9.2vw] md:right-[-48px] top-[-3vw] md:top-[-7px]"
				alt="rel-ring" />
		</div>
		<div v-if="index === 1">
			<NuxtImg :src="ringImg" loading="lazy"
				class="absolute w-[22.95vw] md:w-[115px] h-[22.95vw] md:h-[115px] left-[-6.2vw] md:left-[-30px] top-[-3vw] md:top-[-7px]"
				alt="rel-ring" />
		</div>
		<div v-if="index === 2">
			<NuxtImg :src="ringImg" loading="lazy"
				class="absolute w-[30.4vw] md:w-[150px] h-[30.4vw] md:h-[150px] right-[-12.2vw] md:right-[-59px] top-[-5.2vw] md:top-[-18px]"
				alt="rel-ring" />
		</div>
		<div v-if="index === 3">
			<NuxtImg :src="ringImg" loading="lazy"
				class="absolute w-[25.1vw] md:w-[120px] h-[25.1vw] md:h-[127px] left-[-7.2vw] md:left-[-30px] top-[-1.8vw] md:top-[-2px]"
				alt="rel-ring" />
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'index',
		'titTxt',
		'startColor',
		'endColor',
		'topImg',
		'iPadImg',
		'linkUrl',
		'btnTxt',
		'ringImg',
		'customPadding',
	]
}
</script>
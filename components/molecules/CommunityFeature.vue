<template>
	<div class="flex flex-col justify-between items-center">
		<div class="relative">
			<AtomsHeadTitle2 :text="text" startColor="#55CCAA" endColor="#88DD77" :customCommunityFeature1="customCommunityFeature1" :customCommunityFeature2="customCommunityFeature2" />
		</div>
		<AtomsCard class="rounded-full relative top-[-3vw] md:top-[-15px] z-[-1]">
			<div
				class="flex justify-center items-center text-smtit md:text-tit bg-white rounded-full text-green font-medium w-[22vw] md:w-[110px] h-[22vw] md:h-[110px]">
				{{ tit }}
			</div>
		</AtomsCard>
	</div>
</template>

<script>
export default {
	props: [
		'text',
		'tit',
		'customCommunityFeature1',
		'customCommunityFeature2',
	]
}
</script>
<template>
	<AtomsCard class="flex w-full rounded-[4vw] md:rounded-[20px] relative h-full">
		<div class="w-full flex flex-col p-[2.8vw] md:p-[14px]">
			<span
				class="font-apple text-[#666666] font-light w-full text-[4.8vw] md:text-[24px] absolute top-[3.4vw] md:top-[17px] left-[6vw] md:left-[30px]">Kazuho
				Ishida</span>
			<p class="text-[4vw] md:text-[20px] mb-[2vw] md:mb-[10px] relative z-50">石田 一帆</p>
			<span class="text-smmini md:text-mini">ショップ店員 / 24歳 / </span>
		</div>
		<NuxtImg :src="img" loading="lazy" class="h-[24vw] md:h-[120px] w-[46.7vw] md:w-[276px]" alt="player" />
	</AtomsCard>
</template>

<script>
export default {
	props: [
		'img',
	]
}
</script>

<style scoped></style>
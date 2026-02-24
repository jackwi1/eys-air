<template>
	<div class="relative w-[50vw] md:w-[250px] mx-auto">
		<NuxtImg :src="img" loading="lazy" :class="[customSize || 'w-[24vw] md:w-[120px] h-[22.13vw] md:h-[115px] ml-[14vw] md:ml-[70px]']" alt="article-title" />
		<div class="absolute flex flex-col justify-center items-center left-0 top-0 w-full h-full text-center">
			<p class="text-[4vw] md:text-[20px]">Na-ra-uno 体験記</p>
			<h5 class="text-[5.1vw] md:text-[30px] mt-[2vw] md:mt-[10px] tracking-loose">{{ txt }}</h5>
		</div>
	</div>
</template>

<script>
export default {
	props: [
		'img',
		'txt',
		'customSize',
	]
}
</script>

<style scoped></style>
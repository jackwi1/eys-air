<template>
	<div class="relative">
		<NuxtImg :src="img" loading="lazy" :class="[customSize || 'w-[21.35vw] md:w-[105px] h-[23.5vw] md:h-[117.5px]']" alt="union-img" />
		<p class="absolute left-0 top-0 w-full h-full flex text-center items-center justify-center text-[3.2vw] md:text-[16px] leading-[4vw] md:leading-[20px]"
			v-html="text">
		</p>
	</div>
</template>

<script>
export default {
	props: [
		'img',
		'text',
		'customSize',
	]
}
</script>

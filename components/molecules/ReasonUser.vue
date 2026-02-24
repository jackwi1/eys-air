<template>
	<div class="relative flex flex-col items-center">
		<NuxtImg :src="userImg" loading="lazy" class="w-[25vw] md:w-[125px] h-[26.8vw] md:h-[133.5px]" alt="user-img" />
	</div>
	<div class="bg-white flex flex-col justify-center items-center py-[2vw] md:py-[9.5px] pt-[3vw] md:pt-[15px] pb-[0.8vw] md:pb-[4px] w-full shadow-md"
		:class="[isClicked ? 'active' : '']">
		<p class="text-[5.5vw] md:text-[27.5px] leading-[4.4vw] md:leading-[22px]">{{ text }}</p>
		<span class="text-[2.7vw] md:text-[13.5px] leading-[4.4vw] md:leading-[22px] pt-[0.8vw] md:pt-[4px] ">の場合</span>
	</div>
	<div :class="[isClicked ? 'triangle border-[2.8vw] md:border-[13px] border-b-[0] drop-shadow-md' : '']"></div>
</template>

<script>

export default {
	props: [
		'userImg',
		'text',
		'isClicked'
	]
}
</script>

<style scoped>
.active {
	background-color: #222222;
	color: white;
}

.triangle {
	width: 0px;
	height: 0px;
	border-style: solid;
	border-color: #222222 transparent transparent transparent;
	transform: rotate(0deg);
}
</style>
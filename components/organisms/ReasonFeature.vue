<template>
	<div :class="[customBottom, 'flex flex-col justify-center items-center mb-[2.9vw] md:mb-[13px] relative']">
		<AtomsReasonParallel :text="titTxt" :startColor="startColor" :customTitlePadding="customTitlePadding" :endColor="endColor" />
		<span class="text-[2.5vw] md:text-[14px] pt-[1.5vw] md:pt-[8px] leading-[5vw] md:leading-[24px] tracking-normal">{{ subTxt }}</span>
		<p class="text-[4.3vw] md:text-[21.5px] font-bold leading-[6vw] md:leading-[30px] text-center pb-[2.4vw] md:pb-[12px] tracking-normal" v-html="text">
		</p>
		<NuxtImg :src="imgUrl" loading="lazy" :class="[customImageSetting1, customImageSetting2]" alt="reason-feature" />
		<a :href="linkUrl"
			class="button block absolute left-[50%] md:left-[50.5%] translate-x-[-50%] bottom-[6.5vw] md:bottom-[31px] w-[32vw] md:w-[160px] h-[8vw] md:h-[40px] flex items-center justify-center drop-shadow-[3px_3px_6px_rgba(0,0,0,0.3)]">
			<span class="text-smbase md:text-base">詳細を見る</span>
			<NuxtImg src="/img/arrow.webp" loading="lazy"
				class="inline absolute right-[2vw] md:right-[10px] top-[50%] translate-y-[-50%] w-[3.2vw] md:w-[16px] h-[1.4vw] md:h-[7px]"
				alt="arrow" />
		</a>
	</div>
</template>

<script>
export default {
	props: [
		'index',
		'titTxt',
		'startColor',
		'endColor',
		'subTxt',
		'text',
		'imgUrl',
		'linkUrl',
		'customTitlePadding',
		'customImageSetting1',
		'customImageSetting2',
		'customBottom',
	]
}
</script>

<style scoped>
.button {
	text-decoration: none;
	background-color: #000;
	border: solid 2px #000;
	color: #fff;
	display: block;
	margin: 0 auto;
	text-align: center;
	transition: 0.5s;
}

.btnImg {
	display: inline;
	position: absolute;
	right: 10px;
	top: 50%;
	transform: translateY(-50%);
}

.button:hover {
	color: #fff;
	background: #fff;
	color: #000;
	border: solid 2px #000;
}
</style>
<template>
	<NuxtLink to="/" class="reg-btn flex w-full items-center justify-between px-[4.6vw] md:px-[23px] hover:opacity-75">
		<NuxtImg src="/img/user.webp" loading="lazy" class="w-[5.6vw] md:w-[28px] h-[8vw] md:h-[40px]" alt="user" />
		<div class="py-[1.9vw] md:py-[9px]">
			<p class="text-[#FF6E6E] text-[3.3vw] md:text-[16.5px] tracking-widest">簡易メンバー登録して</p>
			<p class="text-[5vw] md:text-[24px] pt-[2vw] md:pt-[10px] pb-[0.5vw] md:pb-[2.5px] tracking-[1vw] md:tracking-[5px] font-bold">2,000円をGET</p>
		</div>
		<NuxtImg src="/img/arrow.webp" loading="lazy" class="w-[5vw] md:w-[25px] h-[1.8vw] md:h-[9px]" alt="arrow" />
	</NuxtLink>
</template>

<style scoped>
.reg-btn {
	text-decoration: none;
	background-color: #000;
	border: solid 2px #000;
	color: #fff;
	margin: 0 auto;
	text-align: center;
	transition: 0.5s;
	position: relative;
}
</style>
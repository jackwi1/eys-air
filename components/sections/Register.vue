<template>
	<div :class="['relative overflow-x-clip px-[2.6vw] md:px-[13px] z-[1]', maginTop || 'mt-[8vw] md:mt-[5px]']">
		<div
			class="bg-black text-white py-[1.6vw] md:py-[10px] rounded-t-[1.6vw] md:rounded-t-[8px] relative z-10 flex justify-center items-center tracking-normal">
			<span class="text-[4.5vw] md:text-[24px] font-roboto font-bold pr-[1vw] md:pr-[5px] italic">12/14</span>
			<span class="number text-[3.8vw] md:text-[19px] font-bold">23:59</span><span class="jp ml-[1vw] md:ml-[5px]">まで</span>
			<span
				class="bg-white text-[#FF6E6E] py-[1.35vw] md:py-[5px] px-[2.7vw] md:px-[13.5px] text-[4.8vw] md:text-[24px] rounded-[1.6vw] md:rounded-[8px] font-extrabold mx-[0.6vw] md:mx-[3px] ml-[1.7vw] md:ml-[10px]">
				本日締切
			</span>
			<span class="jp">残り</span><span class="number">10</span>
			<span class="jp">時間</span><span class="number">42</span><span class="jp">分</span>
			<span class="number">38</span><span class="jp">秒</span>
		</div>
		<div class="relative">
			<h2 class="text-[6.4vw] md:text-[32px] text-center pt-[4vw] md:pt-[20px] pb-[3vw] md:pb-[15px] font-bold relative z-10 tracking-widest">
				今だけキャンペーン中！
			</h2>
			<div class="relative z-20">
				<div class="px-[4vw] md:px-[20px]">
					<div class="flex justify-start items-center">
						<div class="text-white px-[4.5vw] md:px-[22.5px] py-[1.8vw] md:py-[8px] transform skew-x-[-25deg] font-bold"
							:style="{ background: `linear-gradient(45deg, #FF7273, #FFBCDD)` }">
							<p class="text-[4.4vw] md:text-[22px] transform skew-x-[25deg]">今なら</p>
						</div>
					</div>
					<div class="flex justify-start items-center">
						<div
							class="flex items-center text-white px-[3.2vw] md:px-[15.5px] py-[1.17vw] md:py-[6px] ml-[1.6vw] md:ml-[8px] transform skew-x-[-25deg]"
							:style="{ background: `linear-gradient(45deg, #FF7273, #FFBCDD)` }">
							<NuxtImg src="/img/tick.webp" loading="lazy"
								class="w-[12vw] md:w-[60px] h-[11vw] md:h-[55px] transform skew-x-[25deg]" alt="tick" />
							<span
								class="font-roboto text-[8.8vw] md:text-[44px] transform skew-x-[25deg] px-[1.5vw] md:px-[10px] italic font-bold">2,000</span>
							<span class="text-[4.85vw] md:text-[24.25px] pt-[1vw] md:pt-[14px] transform skew-x-[25deg] font-bold">円OFFチケット</span>
						</div>
					</div>
					<div class="flex justify-end items-center">
						<div class="text-white pr-[2vw] pl-[4.2vw] md:px-[23px] py-[1.65vw] md:py-[9.5px] transform skew-x-[-25deg] font-bold"
							:style="{ background: `linear-gradient(45deg, #FF7273, #FFBCDD)` }">
							<p class="text-[4.8vw] md:text-[22px] transform skew-x-[25deg] tracking-widest">プレゼント！</p>
						</div>
					</div>
				</div>
				<div class="px-[3vw] md:px-[15px] pt-[2.7vw] md:pt-[16px] pb-[0.7vw] md:pb-[3.5px]">
					<AtomsRegisterButton class="relative z-20" />
					<div class="flex justify-center py-[1vw] md:py-[5px]">
						<NuxtLink to="/" class="relative z-20 text-smbase text-[#444444] md:text-base hover:opacity-75 underline">メンバーの方はログイン
						</NuxtLink>
					</div>
				</div>
			</div>
		</div>
		<NuxtImg src="/img/campaign-bg.webp" loading="lazy"
			class="absolute top-0 left-0 z-5 opacity-100 px-[2.6vw] md:px-[13px] h-[80vw] md:h-[400px] w-full drop-shadow-[3px_3px_6px_rgba(0,0,0,0.3)]" alt="campaign-bg" />
	</div>
</template>

<script>
export default {
	props: ['maginTop']
}
</script>

<style scoped>
.number {
	font-size: 4vw;
	font-weight: 700;
	font-family: "Roboto";
	font-style: italic;
	margin-right: 0.6vw;
}

.jp {
	font-size: 2.5vw;
	letter-spacing: 0;
}

@media (min-width: 500px) {
	.number {
		font-size: 20px;
		margin-right: 3px;
	}

	.jp {
		font-size: 14px;
	}
}
</style>
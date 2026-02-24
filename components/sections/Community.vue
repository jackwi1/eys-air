<template>
	<div class="relative overflow-x-clip mt-[0.7vw] md:mt-[4px]">
		<AtomsSectionTitle text="コミュニティ" class="relative z-10 pt-[18vw] md:pt-[90px] pb-[7vw] md:pb-[35px]" />
		<NuxtImg src="/img/community/community-bg.webp" loading="lazy"
			class="absolute w-[99vw] md:w-[495px] h-[80vw] md:h-[400px] left-[-16vw] md:left-[-79px] top-[-18vw] md:top-[-90px]"
			alt="community-bg" />
		<div class="flex justify-center items-end">
			<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]"
				alt="backslash" />
			<h3
				class="text-[4.4vw] md:text-[22px] leading-[6vw] md:leading-[30px] text-center mx-[2.6vw] md:mx-[16px] font-medium ">
				リアルでの出会いを、<br>大切に考えています！
			</h3>
			<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]" alt="slash" />
		</div>

		<div class="flex flex-col mt-[1.5vw] md:mt-[6px] gap-[1vw] md:gap-[4.5px]">
			<div class="relative z-20">
				<MoleculesCommunityFeature text="講師との間に<br>生まれる" tit="絆" class="relative z-10 pt-[3vw] md:pt-[15px] pr-[3vw] md:pr-[15px] " />
				<NuxtImg src="/img/community/feature1.webp" loading="lazy"
					class="w-[48vw] md:w-[240px] h-[48vw] md:h-[240px] absolute bottom-[-30.5vw] md:bottom-[-154px] left-[45.3vw] md:left-[225px]"
					alt="feature1" />
			</div>
			<div class="flex justify-start relative z-20 left-[2.5vw] md:left-[12.5px]">
				<MoleculesCommunityFeature text="趣味を通じて繋がる<br>一生モノの" tit="仲間" customCommunityFeature1="px-[4.1vw] md:px-[23px]"
					class="relative z-10 left-[-2vw] md:left-[-10px]" />
				<NuxtImg src="/img/community/feature2.webp" loading="lazy"
					class="w-[55.2vw] md:w-[276px] h-[55.2vw] md:h-[276px] absolute bottom-[-30.5vw] md:bottom-[-150px] left-[4.8vw] md:left-[22px] z-[7]"
					alt="feature2" />
				<NuxtImg src="/img/community/ring-bg.webp" loading="lazy"
					class="w-[45.4vw] md:w-[227px] h-[45.4vw] md:h-[227px] absolute z-[5] top-[3.6vw] md:top-[18px] left-[0.6vw] md:left-[3px]"
					alt="feature2-ring" />
			</div>
			<div class="flex justify-end relative z-20 right-[-2vw] md:right-[-10px] mt-[1.2vw] md:mt-[6px]">
				<MoleculesCommunityFeature text="レッスン＆飲み会で<br>生まれる" tit="恋愛" class="relative z-10" customCommunityFeature1="px-[4.1vw] md:px-[23px]" />
				<NuxtImg src="/img/community/feature3.webp" loading="lazy"
					class="w-[50.7vw] md:w-[253.5px] h-[50.7vw] md:h-[253.5px] absolute bottom-[-28vw] right-[25vw] md:right-[125px] top-[21.5vw] md:top-[108px] z-[7]"
					alt="feature3" />
				<NuxtImg src="/img/community/ring-bg.webp" loading="lazy"
					class="w-[31.8vw] md:w-[159px] h-[31.8vw] md:h-[159px] absolute z-[5] right-[10.7vw] md:right-[53.5px] top-[24vw] md:top-[120px]"
					alt="ring-bg" />
				<NuxtImg src="/img/community/inner-ring.webp" loading="lazy"
					class="w-[22.2vw] md:w-[111px] h-[22.2vw] md:h-[111px] absolute z-[5] top-[61vw] md:top-[305px] right-[57.1vw] md:right-[285px]"
					alt="inner-ring" />
			</div>
		</div>

		<div class="px-[7vw] md:px-[35px] mt-[39.7vw] md:mt-[198px]">
			<AtomsParallel3 text="ここはあなたの" startColor="#55CCAA" endColor="#88DD77" class="flex justify-start" />
			<AtomsParallel3 text="セカンドコミュニティ" startColor="#55CCAA" endColor="#88DD77" class="flex justify-end" customPadding="px-[3.9vw] md:px-[23.5px]" />
		</div>

		<div class="flex flex-col justify-center items-center mt-[16vw] md:mt-[80px] relative">
			<NuxtImg src="/img/community/logo_EVNTRs.webp" loading="lazy"
				class="w-[50vw] md:w-[250px] h-[8vw] md:h-[40px] mb-[4.7vw] md:mb-[20px]" alt="evntr-logo" />
			<div class="flex justify-center items-end">
				<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]"
					alt="backslash" />
				<h3 class="text-[4.5vw] md:text-[23px] text-center mx-[2.9vw] md:mx-[14.5px] font-bold leading-snug">
					EVNTRs（イベンターズ）が、<br>四季折々のイベントを企画！
				</h3>
				<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7.5px]" alt="slash" />
			</div>
			<NuxtImg src="/img/community/evntrs-ring.webp" loading="lazy"
				class="absolute left-[-12vw] md:left-[-60px] top-[-19vw] md:top-[-93px] w-[32vw] md:w-[160px] h-[32vw] md:h-[160px]"
				alt="evntrs-ring" />

			<NuxtImg src="/img/community/EVNTR.webp" loading="lazy" class="w-full mt-[3.8vw] md:mt-[22px]" alt="EVNTR" />

			<div class="p-[3vw] md:p-[15px]">
				<AtomsHeadTitle3 text="世代・性別・国籍・仕事...<br>バリエーション豊かな仲間が集います！" startColor="#55CCAA" endColor="#88DD77"
					class="relative top-[-11vw] md:top-[-55px]" />
				<div class="flex flex-wrap justify-between gap-y-[2.6vw] md:gap-y-[12px] relative top-[-5.8vw] md:top-[-30px]">
					<NuxtImg src="/img/community/evntrs-ring.webp" loading="lazy"
						class="absolute w-[14vw] md:w-[70px] h-[14vw] md:h-[70px] top-[-2.4vw] md:top-[-12px] left-[-5vw] md:left-[-25px]"
						alt="evntrs-ring" />

					<MoleculesEVNTRCard img="/img/community/EVNTR1.webp" tit="お花見" class="w-[32%] relative z-10" />
					<MoleculesEVNTRCard img="/img/community/EVNTR2.webp" tit="船上パーティー" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/community/EVNTR3.webp" tit="海水浴ライブ" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/community/EVNTR4.webp" tit="餅つき大会" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/community/EVNTR5.webp" tit="秋のBBQ" class="w-[32%]" />
					<MoleculesEVNTRCard img="/img/community/EVNTR6.webp" tit="ハロウィンパーティー" class="w-[32%] relative z-10" />

					<NuxtImg src="/img/community/evntrs-ring.webp" loading="lazy"
						class="absolute w-[22.2vw] md:w-[110px] h-[22.2vw] md:h-[110px] right-[-7.5vw] md:right-[-40px] bottom-[-7.3vw] md:bottom-[-40px]"
						alt="evntrs-ring" />
				</div>
			</div>

			<div class="w-full relative top-[-1vw] md:top-[-6px]">
				<AtomsHeadTitle3 text="PICK UP！<br>こんなイベントを開催中！" startColor="#55CCAA" endColor="#88DD77" customPadding="px-[3.95vw] md:px-[19.5px]"/>
				<Swiper :slides-per-view="2" :effect="'creative'" :creative-effect="{
					prev: {
						translate: ['-20%', 0, 0],
					},
					next: {
						translate: ['100%', 0, 0],
					},
				}" :initial-slide="1" :centered-slides="true">
					<SwiperSlide class="px-[2vw] md:px-[10px]">
						<div class="flex flex-col items-center py-[5vw] md:py-[20px] justify-center">
							<p class="font-roboto text-smlarge md:text-large">11.16</p>
							<span
								class="font-roboto font-medium text-[4vw] md:text-[20px] tracking-[3vw] md:tracking-[15px] pl-[3vw] md:pl-[15px]">Fri</span>
							<div class="flex justify-evenly my-[4.8vw] md:my-[26px] w-full">
								<span
									class="text-[#05B0FD] text-[2.7vw] md:text-[13px] bg-white px-[1vw] md:px-[5px] rounded-full">申込受付中</span>
								<span
									class="text-[#FF8822] text-[2.7vw] md:text-[13px] bg-white px-[1vw] md:px-[5px] rounded-full">残席わずか：2席</span>
							</div>
							<NuxtImg src="/img/community/slider1.webp" loading="lazy"
								class="w-[44vw] md:w-[220px] h-[44vw] md:h-[220px]" alt="community1" />
							<MoleculesPickUp tit="VEGAS NIGHT" avatar="/img/community/avatar1.webp" color="#2FBD9A"
								school="EYS Music School" desc="綺羅びやかなショート白熱のカジノ、誰しもが憧れる非日常体験の街、ラスベガス。そんなラスベガスの夜をテーマにした指フェスを開催！"
								price="3,000円" startColor="#798DEF" endColor="#92C9EF" linkUrl="/" />
						</div>
					</SwiperSlide>

					<SwiperSlide class="px-[2vw] md:px-[10px]">
						<div class="flex flex-col items-center py-[5vw] md:py-[20px] justify-center">
							<p class="font-roboto text-smlarge md:text-large">11.18</p>
							<span
								class="font-roboto font-medium text-[4vw] md:text-[20px] tracking-[3vw] md:tracking-[15px] pl-[3vw] md:pl-[15px]">Sun</span>
							<div class="flex my-[4.8vw] md:my-[26px]">
								<span
									class="text-[#FF4444] text-[2.7vw] md:text-[13px] bg-white px-[1vw] md:px-[5px] rounded-full">満員御礼</span>
							</div>

							<NuxtImg src="/img/community/slider2.webp" loading="lazy"
								class="w-[44vw] md:w-[220px] h-[44vw] md:h-[220px]" alt="community2" />

							<MoleculesPickUp tit="星空キャンプ" avatar="/img/community/avatar2.webp" color="#2FBD9A" school="Wataru"
								desc="日頃の仕事を忘れて、山の上へ。満点の星空の中、普段言えないこと、話してみませんか。初心者大歓迎！キャンピング用品シェア中。" price="1,000円" startColor="#DDD"
								endColor="#DDD" linkUrl="/" />
						</div>
					</SwiperSlide>

					<SwiperSlide class="px-[2vw] md:px-[10px]">
						<div class="flex flex-col items-center py-[5vw] md:py-[20px] justify-center">
							<p class="font-roboto text-smlarge md:text-large">11.19</p>
							<span
								class="font-roboto font-medium text-[4vw] md:text-[20px] tracking-[3vw] md:tracking-[15px] pl-[3vw] md:pl-[15px]">Mon</span>
							<div class="flex justify-evenly my-[4.8vw] md:my-[26px] w-full">
								<span
									class="text-[#05B0FD] text-[2.7vw] md:text-[13px] bg-white px-[1vw] md:px-[5px] rounded-full">申込受付中</span>
								<span
									class="text-[#FF8822] text-[2.7vw] md:text-[13px] bg-white px-[1vw] md:px-[5px] rounded-full">残席わずか：2席</span>
							</div>

							<NuxtImg src="/img/community/slider3.webp" loading="lazy"
								class="w-[44vw] md:w-[220px] h-[44vw] md:h-[220px]" alt="community3" />

							<MoleculesPickUp tit="ピアノ・デュオの宴" avatar="/img/community/avatar3.webp" color="#38AEDA"
								school="EYS Music School" desc="綺羅びやかなショート白熱のカジノ、誰しもが憧れる非日常体験の街、ラスベガス。そんなラスベガスの夜をテーマにした指フェスを開催！"
								price="無料" startColor="#798DEF" endColor="#92C9EF" linkUrl="/" />
						</div>
					</SwiperSlide>
				</Swiper>

				<div class="flex justify-center w-[53.34%] mx-auto mt-[2.3vw] md:mt-[17px]">
					<AtomsComButton btnText="イベント一覧" linkUrl="/" imgUrl="/img/arrow.webp" />
				</div>
			</div>
		</div>
	</div>
</template>

<!-- <script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const showElement = ref(false)

const handleScroll = () => {
	if (window.scrollY > 1000) {
		showElement.value = true
	} else {
		showElement.value = false
	}
}

onMounted(() => {
	window.addEventListener('scroll', handleScroll)
})

onUnmounted(() => {
	window.removeEventListener('scroll', handleScroll)
})
</script> -->
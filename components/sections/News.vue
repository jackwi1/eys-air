<template>
	<div class="relative overflow-x-clip z-10">
		<AtomsSectionTitle text="新着トピックス" class="relative z-10 pt-[20vw] md:pt-[104px] pb-[13vw] md:pb-[60px]" />
		<NuxtImg src="/img/news/news-bg.webp" loading="lazy"
			class="absolute w-[80vw] md:w-[400px] h-[80vw] md:h-[400px] left-[-16vw] md:left-[-80px] top-[-16vw] md:top-[-77px]"
			alt="news" />
		<NuxtImg src="/img/news/news-ring.webp" loading="lazy"
			class="absolute w-[31vw] md:w-[160px] h-[31vw] md:h-[160px] right-[-8.5vw] md:right-[-47px] top-[26.5vw] md:top-[131px]"
			alt="news-ring" />
		<div>
			<Swiper class="news-swiper" :slides-per-view="1.3" :effect="'creative'" :creative-effect="{
				prev: {
					translate: ['-100%', 0, 0],
				},
				next: {
					translate: ['100%', 0, 0],
				},
			}">
				<SwiperSlide>
					<AtomsCard class="w-[65vw] md:w-[325px] rounded-md">
						<OrganismsNewsCard text="新規OPEN" startColor="#FF4455" endColor="#FF99EE" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[65vw] md:w-[325px] rounded-md">
						<OrganismsNewsCard text="発表会 [ユビフェス]" startColor="#00CCEE" endColor="#44EECC" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[65vw] md:w-[325px] rounded-md">
						<OrganismsNewsCard text="イベント" startColor="#00BBBB" endColor="#66EEBB" />
					</AtomsCard>
				</SwiperSlide>

				<SwiperSlide>
					<AtomsCard class="w-[65vw] md:w-[325px] rounded-md">
						<OrganismsNewsCard text="バンド" startColor="#0088EE" endColor="#66CCFF" />
					</AtomsCard>
				</SwiperSlide>
			</Swiper>
		</div>
		<div class="px-[5.4vw] md:px-[27px] mt-[-1.5vw] md:mt-[-7.5px]">
			<AtomsCard class="my-[5.9vw] md:my-[27px] rounded-md">
				<OrganismsEYSDesc />
			</AtomsCard>
			<AtomsCard class="rounded-md mt-[-2vw] md:mt-[10px]">
				<OrganismsEYSAll />
			</AtomsCard>
		</div>
	</div>
</template>

<style scoped>
.news-swiper {
	padding-left: 5.4vw;
}

@media (min-width: 500px) {
	.news-swiper {
		padding-left: 27px;
	}
}
</style>
<template>
	<div class="relative overflow-x-clip top-[-31.5vw] md:top-[-225px] mb-[-26vw] md:mb-[-198px] z-10">
		<NuxtImg src="/img/joinus/join-ring.webp" loading="lazy"
			class="absolute w-[30vw] md:w-[150px] h-[32vw] md:h-[158px] left-[-13vw] md:left-[-65px] top-[7.2vw] md:top-[39px]"
			alt="join-ring" />
		<NuxtImg src="/img/joinus/join-bg.webp" loading="lazy"
			class="absolute w-[93vw] md:w-[465px] h-[80vw] md:h-[400px] right-[-21vw] md:right-[-106px] top-[-31vw] md:top-[-152px]"
			alt="join-bg" />
		<AtomsSectionTitle text="EYS air の始め方" class="relative z-10" />

		<div class="flex justify-center items-end">
			<NuxtImg src="/img/backslash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7px]"
				alt="backslash" />
			<h3 class="text-[4.3vw] md:text-[22px] text-center mx-[2.5vw] md:mx-[10px] font-medium mt-[7vw] md:mt-[35px] tracking-widest leading-snug font-bold">
				お申し込み〜利用までは、<br>カンタン3STEP！
			</h3>
			<NuxtImg src="/img/slash.webp" loading="lazy" class="w-[4.4vw] md:w-[22px] h-[7vw] md:h-[35px] mb-[1.5vw] md:mb-[7px]" alt="slash" />
		</div>

		<div class="px-[5.4vw] md:px-[27px] mt-[4.4vw] md:mt-[22px] relative">
			<MoleculesJoinStep step="STEP 1" , tit='簡易メンバー登録して、<br>入会金2,000円OFFチケットをゲット'
				desc="カンタンな登録情報を入力して、<br>アカウント作成するだけ！" img="/img/joinus/join1.webp" class="relative z-10" />
			<MoleculesJoinStep step="STEP 2" , tit='豊富なジャンルから、<br>気になるコースを予約' desc="音楽・ワイン・茶道・陶芸...<br>お好きなジャンルを自由にチョイス！"
				img="/img/joinus/join2.webp" class="relative z-10" />
			<MoleculesJoinStep step="STEP 3" , tit='オンラインで気軽に<br>レッスンを受講' desc="レッスン開始5分前に<br>入室ボタンを選択してスタート！"
				img="/img/joinus/join3.webp" class="relative z-10" />
			<NuxtImg src="/img/joinus/join-ring.webp" loading="lazy"
				class="absolute w-[19vw] md:w-[95px] h-[19vw] md:h-[95px] right-[1vw] md:right-[5px] bottom-[-9vw] md:bottom-[-45px]"
				alt="join-ring" />
		</div>

		<div class="px-[5.4vw] md:px-[27px] mt-[24.5vw] md:mt-[118px]">
			<NuxtImg src="/img/joinus/logo.webp" loading="lazy" class="w-full h-[20vw] md:h-[100px]" alt="join-logo" />
			<OrganismsPageItem :index="currentIndex" :totalPosts="totalPosts" />
			<div class="pagination flex justify-center mt-[20vw] md:mt-[103.5px]">
				<vue-awesome-paginate :total-items="totalPosts" :items-per-page="1" v-model="currentPage"
					:max-pages-shown="3" />
			</div>
		</div>

		<div class="px-[5.4vw] md:px-[27px] mt-[13.5vw] md:mt-[80px] flex flex-col gap-y-[20px] md:gap-y-[28px]">
			<AtomsArticleTitle img="/img/joinus/article/title.webp" txt="人気の記事" class="mb-[2.8vw] md:mb-[10px]"/>
			<AtomsArticle img="/img/joinus/article/01.webp" />
			<AtomsArticle img="/img/joinus/article/02.webp" />
			<AtomsArticle img="/img/joinus/article/03.webp" />
		</div>

		<div class="px-[5.5vw] md:px-[27px] mt-[10vw] md:mt-[79px] flex flex-col gap-y-[20px] md:gap-y-[27px]">
			<AtomsArticleTitle img="/img/joinus/player/title.webp" txt="人気のプレイヤー" class="mb-[1.6vw] md:mb-[-20px] top-[-2vw] md:top-[-38px]" customSize="w-[15.57vw] md:w-[76px] h-[24.16vw] md:h-[120px] ml-[19vw] md:ml-[95px]" />
			<AtomsPlayer img="/img/joinus/player/01.webp" />
			<AtomsPlayer img="/img/joinus/player/02.webp" />
			<AtomsPlayer img="/img/joinus/player/03.webp" />
			<AtomsPlayer img="/img/joinus/player/04.webp" />
		</div>
	</div>
</template>

<script lang="ts" setup>
import { ref, computed } from 'vue';
const currentPage = ref(1);

const totalPosts = computed(() => {
	return 3;
});

const currentIndex = computed(() => {
	return currentPage.value;
})

</script>


<style scoped>
.pagination {
	width: 100%;
	padding: 10px 0;
}
</style>
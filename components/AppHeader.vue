<template>
	<header>
		<div class="menu-bar flex flex-col fixed top-0 w-full max-w-[500px] border-[0.5px] border-[#DDDDDD] z-[9999]"
			:class="navIsOpen ? 'scrollbar h-screen min-h-full overflow-y-auto bg-black' : ''">
			<div class="flex justify-between border-b-[0.5px] border-[#DDDDDD] p-[2.4vw] md:p-[12px]"
				:class="[navIsOpen ? 'bg-[#4A4A4A]' : 'bg-white']">
				<NuxtLink to="/" class="flex items-center">
					<NuxtImg :src="navIsOpen ? '/img/logo_air_clicked.webp' : '/img/logo_air.webp'" loading="lazy"
						class="w-[37vw] md:w-[185px] h-[8.8vw] md:h-[44px]" alt="Logo" />
					<span class="text-smtiny md:text-tiny ml-[3vw] md:ml-[12px]"
						:class="[navIsOpen ? 'text-white' : 'text-[#222222]']">オンラインアカデミー</span>
				</NuxtLink>
				<button @click="toggleNav" class="flex flex-col justify-center relative" aria-label="hamburger_menu">
					<span class="w-[5.4vw] md:w-[27px] h-[0.4vw] md:h-[2px] mt-[-0.3vw] md:mt-[-3px] transition-all duration-300 ease-linear"
						:class="navIsOpen ? 'translate-y-[1.7vw] md:translate-y-[8.5px] rotate-[45deg] bg-white origin-center' : 'origin-left bg-[#000000]'">
					</span>
					<span
						class="w-[5.4vw] md:w-[27px] h-[0.4vw] md:h-[2px] mt-[2.9vw] md:mt-[14px] transition-all duration-300 ease-linear"
						:class="navIsOpen ? 'translate-y-[-1.7vw] md:translate-y-[-8.5px] -rotate-[45deg] bg-white origin-center' : 'origin-left bg-[#000000]'">
					</span>
				</button>
			</div>
			<div v-if="navIsOpen">
				<OrganismsMenuList />
			</div>
		</div>
	</header>
</template>

<script lang="ts" setup>
const navIsOpen = useState('navIsOpen', () => false);

function toggleNav(event: MouseEvent): void {
	event.preventDefault();
	navIsOpen.value = !navIsOpen.value;
}
</script>

<style scoped>
.menu-bar {
	left: 0;
}

@media (min-width: 500px) {
	.menu-bar {
		left: calc(50% - 250px); 
	}
}
</style>
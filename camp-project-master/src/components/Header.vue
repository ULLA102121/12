<script setup>
import {ArrowRightIcon, ChevronDoubleDownIcon} from '@heroicons/vue/solid'
</script>
<template>
	<section class="bg-orange-200 flex flex-col justify-center items-center md:px-20 min-h-screen">
		<div class="flex flex-col w-full py-12 px-4 lg:px-0 justify-center items-end">
			<p class="text-3xl text-orange-800 font-extrabold">哈囉！我是<span class="text-orange-800">施淳瑜</span></p>
			<h1 class="text-5xl text-right text-red-600 mt-1 font-extrabold">
				一個喜歡吃美食的高中生
			</h1>
			<p class="text-3xl text-red-700 font-medium pt-8">
				[食物介紹]
			</p>
			<a
				href="#contact"
				class="mt-3 flex items-center text-xl font-regular pb-3">
				聯絡我
				<ArrowRightIcon class="ml-1 w-8 h-5"/>
			</a>
		</div>

		<a href="#activities" class="animate-bounce cursor-pointer">
			<chevron-double-down-icon class="w-18 h-16"/>
		</a>
	</section>
</template>

<script setup>
import {ArrowRightIcon} from "@heroicons/vue/outline";

const skills = [
	{
		title: '珍珠奶茶',
		description: '冰涼濃厚的奶茶搭配上富含嚼勁的珍珠。',
	},
	{
		title: '芒果雪花冰',
		description: '綿密的牛奶冰屑淋上滿滿的芒果醬與新鮮的芒果塊',
	},
	{
		title: '薯條',
		description: '果然被油炸得金黃的薯條最能擄獲我的舌頭,再怎麼油都無所謂',
	},
	{
		title: '壽司',
		description: '炙燒原味都好吃',
	},
	{
		title: '泡麵',
		description: '便宜又好吃,cp直很高',
	},
]
</script>

<template>

	<section id="about" class="pt-32 md:px-16 bg-gray-800">
		<div class="flex flex-col md:flex-row justify-between items-center md:px-8 md:mb-4">
			<h1 class="text-2xl md:text-4xl text-white font-bold">
				關於食物
			</h1>
			<button
				class="my-8 mr-3 border-b border-red-200 pb-2 flex items-center text-xl text-white">
				所有經歷
				<ArrowRightIcon class="ml-1 w-5 h-5"/>
			</button>
		</div>
		<div class="flex flex-wrap justify-start">
			<div
				class="w-full md:w-1/3"
				v-for="skill in skills">
				>
				<div
					class="px-10 sm:px-20 py-3 sm:py-6 shadow-lg w-11/12 mx-auto bg-white rounded z-20 relative">
					<h4 class="text-orange-400 text-lg text-center mb-2">{{ skill.title }}</h4>
					<p class="text-orange-400 text-lg text-center mb-2">{{ skill.description }}</p>
				</div>
			</div>
		</div>
	</section>
</template>
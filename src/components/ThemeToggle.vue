<script setup lang="ts">

let root = document.querySelector('html')

function toggle() {
	console.log('toggle theme');
	root?.classList.toggle('dark')
}

</script>

<template>
	<button
		@click="toggle"
		class="
		flex flex-row justify-end dark:justify-start items-center
		rounded-full
	bg-togglelight dark:bg-gradient-to-r dark:from-togglegrad1 dark:to-togglegrad2
		h-8 w-16 lg:ml-4 lg:px-1 hover:cursor-pointer
		">
		<div class="circle bg-white dark:bg-darkCardBg h-6 w-6 rounded-full"></div>
		<span class="sr-only">Toggle Dark or Light Theme</span>
	</button>
</template>
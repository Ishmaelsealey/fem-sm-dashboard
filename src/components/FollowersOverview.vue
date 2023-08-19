<template>
	<div class="flex flex-col items-center bg-lightCardBg dark:bg-darkCardBg rounded-lg overflow-hidden">
		<slot name="top-color"/>
		<!-- <div class="h-1.5 w-full mb-3 bg-facebook"></div> -->
		<div class="my-7 font-bold text-darkGrayBlue dark:text-darkText">
			<slot name="icon"/>
			<slot name="username"/>
		</div>
		<h2 class="text-6xl font-bold mb-2 dark:text-white">
			<slot name="follower-count"></slot>
		</h2>
		<div class="tracking-widest uppercase text-darkGrayBlue dark:text-darkText"><slot name="followorsub"/></div>
		<div class="my-6"><slot name="up-down-icon"/> <slot name="up-down-count"/></div>
	</div>
</template>

<template>
	<div class="bg-lightCardBg dark:bg-darkCardBg rounded-lg flex flex-col p-6">
		<div class="flex flex-row justify-between font-bold text-darkGrayBlue dark:text-darkText">
			<slot name="cardTitle"/>
			<slot name="cardIcon"/>
		</div>
		
		<div class="flex flex-row justify-between items-end mt-8">
			<strong class="font-bold text-4xl dark:text-white">
				<slot name="statNum"/>
			</strong>

			<span>
				<span class="mr-1">
					<slot name="statupdownicon"/>
				</span>
				<slot name="statupdownnum"/>
			</span>
		</div>
	</div>
</template>
<script setup lang="ts">
import FollowersOverview from './components/FollowersOverview.vue'
import IconFb from './components/icons/IconFb.vue'
import IconIg from './components/icons/IconIg.vue'
import IconYoutube from './components/icons/IconYoutube.vue'
import IconUp from './components/icons/IconUp.vue'
import IconDown from './components/icons/IconDown.vue'
import IconTwitter from './components/icons/IconTwitter.vue'
import ViewsLikes from './components/ViewsLikes.vue'
import ThemeToggle from './components/ThemeToggle.vue'
</script>

<template>
	<div class="absolute z-0 w-full h-80 bg-lightTopBg dark:bg-darkTopBg rounded-b-3xl lg:rounded-none"></div>
	<div class="grid gap-6 sm:grid-cols-2 lg:grid-cols-4 px-5 pt-10 relative z-10 max-w-7xl mx-auto">
		<div class="col-span-full">
			<h1 class="text-2xl font-bold text-veryDarkBlue dark:text-white">Social Media Dashboard</h1>
			<p class="mb-4 font-bold text-darkGrayBlue dark:text-darkText">Total Followers: 23,004</p>
			<hr class="lg:hidden text-darkGrayBlue dark:text-darkText h-[1px]">
			<div class="flex flex-row lg:justify-end justify-between items-center text-darkGrayBlue dark:text-darkText py-8 lg:py-0
			lg:absolute lg:top-16 lg:right-10">
				<span class="font-bold">Dark Mode</span>
				<ThemeToggle/>
			</div>
		</div>
		<FollowersOverview>
			<template #top-color><div class="h-1.5 w-full bg-facebook"></div></template>
			<template #icon><IconFb/></template>
			<template #username>@nathanf</template>
			<template #follower-count>1987</template>
			<template #followorsub>followers</template>
			<template #up-down-icon><IconUp/></template>
			<template #up-down-count><span class="text-limegreen font-bold">12 Today</span></template>
		</FollowersOverview>
		<FollowersOverview>
			<template #top-color><div class="h-1.5 w-full bg-twitter"></div></template>
			<template #icon>
				<IconTwitter/>
			</template>
			<template #username>@nathanf</template>
			<template #follower-count>1044</template>
			<template #followorsub>followers</template>
			<template #up-down-icon><IconUp/></template>
			<template #up-down-count><span class="text-limegreen font-bold">99 Today</span></template>
		</FollowersOverview>
		<FollowersOverview>
			<template #top-color>
				<div class="h-1.5 w-full bg-gradient-to-r from-instagram1 to-instagram2"></div></template>
			<template #icon><IconIg/></template>
			<template #username>@realnathanf</template>
			<template #follower-count>11k</template>
			<template #followorsub>followers</template>
			<template #up-down-icon><IconUp/></template>
			<template #up-down-count><span class="text-limegreen font-bold">1099 Today</span></template>
		</FollowersOverview>
		<FollowersOverview>
			<template #top-color><div class="h-1.5 w-full bg-youtube"></div></template>
			<template #icon><IconYoutube/></template>
			<template #username>Nathan F.</template>
			<template #follower-count>8239</template>
			<template #followorsub>subscribers</template>
			<template #up-down-icon><IconDown/></template>
			<template #up-down-count><span class="text-brightred font-bold">144 Today</span></template>
		</FollowersOverview>

		<h3 class="col-span-full text-slate-500 font-bold mt-2 text-xl text-darkGrayBlue dark:text-white">
			Overview - Today
		</h3>

		<ViewsLikes>
			<template #cardTitle>Page Views</template>
			<template #cardIcon><IconFb/></template>
			<template #statNum>87</template>
      <template #statupdownicon><IconUp/></template>
      <template #statupdownnum><span class="text-limegreen font-bold">3%</span></template>
    </ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Likes</template>
      <template #cardIcon><IconFb/></template>
      <template #statNum>52</template>
      <template #statupdownicon><IconDown/></template>
      <template #statupdownnum><span class="text-brightred font-bold">2%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Likes</template>
      <template #cardIcon><IconIg/></template>
      <template #statNum>5462</template>
      <template #statupdownicon><IconUp/></template>
      <template #statupdownnum><span class="text-limegreen font-bold">2257%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Profile Views</template>
			<template #cardIcon><IconIg/></template>
			<template #statNum>52k</template>
			<template #statupdownicon><IconUp/></template>
			<template #statupdownnum><span class="text-limegreen font-bold">1375%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Retweets</template>
			<template #cardIcon><IconTwitter/></template>
			<template #statNum>117</template>
			<template #statupdownicon><IconUp/></template>
			<template #statupdownnum><span class="text-limegreen font-bold">303%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Likes</template>
			<template #cardIcon><IconTwitter/></template>
			<template #statNum>507</template>
			<template #statupdownicon><IconUp/></template>
			<template #statupdownnum><span class="text-limegreen font-bold">553%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Likes</template>
			<template #cardIcon><IconYoutube/></template>
			<template #statNum>107</template>
			<template #statupdownicon><IconDown/></template>
			<template #statupdownnum><span class="text-brightred font-bold">19%</span></template>
		</ViewsLikes>
		<ViewsLikes>
			<template #cardTitle>Total Views</template>
			<template #cardIcon><IconYoutube/></template>
			<template #statNum>1407</template>
			<template #statupdownicon><IconDown/></template>
			<template #statupdownnum><span class="text-brightred font-bold">12%</span></template>
		</ViewsLikes>
	</div>
</template>
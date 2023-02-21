<template>
	<v-app>
		<div style="background-color: #F9ECFF;">

		<ApplicationBar/>
		<SideMenu/>

		</div>
	</v-app>
</template>

<script>

import ApplicationBar from '@/components/ApplicationBar.vue';
import SideMenu from '@/components/SideMenu.vue';

export default {
	name: 'App',
	data: () => ({
	}),
	components: {
		ApplicationBar,
		SideMenu
	},
	methods: {

	}
}
</script>

<style>

</style>
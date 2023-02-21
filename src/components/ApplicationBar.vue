<template>
  <div class="d-flex" style="background-color: #F9ECFF;">
    <v-icon 
      size="x-large"
      class="ml-6 mt-4" 
      icon="mdi-vuetify"
      color="#9558DE"
    >
    </v-icon>
    <v-spacer></v-spacer>
    <v-btn
      dense
      variant="plain"
      size="x-large"
      class="" 
      icon="mdi-weather-night"
      color="#9558DE"
    >
    </v-btn>
    <v-btn
      dense
      variant="plain"
      size="x-large"
      class="" 
      icon="mdi-bell-outline"
      color="#9558DE"
    >
    </v-btn>
    <v-btn 		
      dense		
      variant="plain"
      size="x-large"
      class="mr-5"
      icon="mdi-logout"
      color="#9558DE"
     >
    </v-btn>
  </div>
</template>

<script>


export default {
	name: 'App',
	data: () => ({
		//
	}),
	components: {
	}
}
</script>

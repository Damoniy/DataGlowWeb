<template>
    <div class="d-flex flex-column" style="height:92vh; width: 12vw; background-color: #F9ECFF;">	
        <v-divider class="ml-4"></v-divider>
        <v-card 
            v-for="item in this.items" 
            :key="item.id" 
            @click="this.selected = item.id" 
            class="mx-6 pl-2 py-1 d-flex"
            :class="[this.selected === item.id ? 'focused' : 'normal']"
            rounded="lg"
            variant="plain"
        >	
        <div 
            class="my-2 ml-2"
            style="border-radius: 8px;"
            :class="[this.selected === item.id ? 'card-focused' : 'card-normal']"
        >
            <v-icon class="px-4 py-4" size="small" :icon="item.icon" :color="this.selected === item.id ? '#fff' : '#000'"></v-icon>
        </div>	
        <span class="mt-4 ml-2" style="font-size: 12px;">{{ item.title }}</span>

        </v-card>
    </div>
</template>

<script>

    export default {
        data: () => ({
            active: true,
            items: [	
                        {id: 1, title: 'Home', 	icon: 'mdi-home', clicked: false}, 
                        {id: 2, title: 'Configurations', icon: 'mdi-cog-outline', clicked: false},
                        {id: 3, title: 'Profile', icon: 'mdi-account' ,clicked: false}
                    ],
            selected: 0
        }),
    }

</script>

<style>
	.normal {
	}	

	.focused {
		-webkit-box-shadow: 1px 5px 70px -20px rgba(0,0,0,0.75);
		-moz-box-shadow: 1px 5px 70px -20px rgba(0,0,0,0.75);
		box-shadow: 1px 5px 70px -20px rgba(0,0,0,0.75);
	}

	.card-normal {
		background-color: white;
	}

	.card-focused {
		background-color: blueviolet;
	}
</style>
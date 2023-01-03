<template>

    <div class="flex">
        <SidebarComponent></SidebarComponent>
        <div class="flex-1">
            <div class="w-full py-[20px] shadow-sm bg-white">
                <TopbarComponent></TopbarComponent>
            </div>
            <div class="shadow-sm h-full bg-gray-50">
                <router-view></router-view>
            </div>

        </div>
    </div>
    <!-- <div class="flex bg-gray-100">
        <div class="bg-white shadow-sm border min-h-screen duration-200 relative"
            :class="`${sideToggle == true ? 'w-[80px]' : 'w-[300px]'}`">

            <div class="absolute top-[10px] right-[-16px] bg-white shadow h-[30px] w-[30px] rounded-full flex justify-center items-center"
                @click="sidebarToggle()">
                <i class="fa-sharp fa-solid fa-arrow-right-long transition-all delay-150"
                    :class="`${sideToggle == false ? 'rotate-180' : 'rotate-360'}`"></i>
            </div>

            <div class="py-[10px] justify-center inline-flex items-center bg-red-200 w-full">
                <img class="h-[40px] w-[40px]" :class="`${sideToggle == true ? 'block m-auto' : ''}`" src="/favicon.ico" alt="">
                <h1 :class="`pl-3 font-bold text-[18px] ${sideToggle == true ? 'scale-0' : ''}`">logo Here</h1>
            </div>

            <SidebarComponent></SidebarComponent>
        </div>
        <div class="flex-1">
            <div class="w-full py-[20px] shadow-sm bg-white">
                <TopbarComponent></TopbarComponent>
            </div>
            <div class="p-2 bg-white min-h-screen m-3">
                <router-view />
            </div>

        </div>
    </div> -->

</template>

<script>
import SidebarComponent from './components/inc/SidebarComponent.vue'
import TopbarComponent from './components/inc/TopbarComponent.vue'


export default {
    components: { SidebarComponent, TopbarComponent },

    data() {
        return {
            sideToggle: false,
            menuDropDownToggle: false,
        }
    },

    methods: {
        sidebarToggle() {
            this.sideToggle = !this.sideToggle

        },

        menuDropDown() {
            this.menuDropDownToggle = !this.menuDropDownToggle
        }
    }

}

</script>

<style scoped>

</style>
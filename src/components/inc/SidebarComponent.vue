<template>
    <div class="bg-[#2C3A40] h-[100%] px-4  pt-8 relative duration-300 rounded-3xl md:block hidden" :class="`${sideToggle == true ? 'w-[95px]' : 'w-72'}`">
        <div class="absolute top-[10px] right-[-16px] bg-[#00C3FF] h-[30px] w-[30px] rounded-full flex justify-center items-center"
            @click="sidebarToggle()">
            <i class="fa-sharp fa-solid fa-arrow-right-long duration-300 text-white"
                :class="`${sideToggle == false ? 'rotate-180' : 'rotate-360'}`"></i>
        </div>

        <div class="">
            <div class="inline-flex gap-x-3 items-center">
                <div class="float-left">
                    <svg xmlns="http://www.w3.org/2000/svg" width="45" height="45" fill="currentColor"
                        class="bi bi-amd bg-[#00C3FF] p-2 rounded-md duration-300 text-white"
                        :class="`${sideToggle == true ? 'rotate-[360deg]' : ''}`" viewBox="0 0 16 16">
                        <path
                            d="m.334 0 4.358 4.359h7.15v7.15l4.358 4.358V0H.334ZM.2 9.72l4.487-4.488v6.281h6.28L6.48 16H.2V9.72Z" />
                    </svg>
                </div>
                <div class="">
                    <h1 class="text-2xl duration-300 text-white" :class="`${sideToggle == true ? 'scale-0' : ''}`">Tailwind</h1>
                </div>
            </div>

            <div class="flex items-center rounded-md bg-gray-200 py-2 mt-6 px-4">
                <i class="fa-solid fa-magnifying-glass duration-300"
                    :class="`${sideToggle == true ? 'ml-[-8px]' : ''}`"></i>
                <input type="text" class="bg-transparent w-full outline-none focus:outline-none px-3 duration-300"
                    :class="`${sideToggle == true ? 'scale-0' : 'block'}`">

            </div>

            <div class="py-2">
                <ul class="flex flex-col py-3">
                    <li class="mb-2 hover:text-[]">
                        <div class="flex items-center rounded-md bg-[#00C3FF] hover:bg-gray-200 py-2 px-4 gap-x-2">
                            <i class="fa-solid fa-house-user duration-300 text-white"
                                :class="`${sideToggle == true ? 'ml-[-8px]' : ''}`"></i>
                            <span class="text-[1rem] font-medium duration-300 text-white"
                                :class="`${sideToggle == true ? 'scale-0' : ''}`">Home</span>
                            <div class="flex-1 text-right duration-300"
                                :class="`${sideToggle == true ? 'scale-0' : ''}`">
                                <i id="icon" class="fa-solid fa-angle-down duration-300 text-white"
                                    :class="`${menuDropDownToggle == true ? 'rotate-180' : ''}`"
                                    @click="menuDropDown()"></i>
                            </div>
                        </div>

                        <div class="pl-5 py-2 duration-300" :class="`${menuDropDownToggle == true ? 'show' : 'hide'}`">
                            <ul>
                                <li>item 01</li>
                                <li>item 01</li>
                                <li>item 01</li>
                                <li>item 01</li>
                            </ul>
                        </div>
                    </li>
                    <li class="mb-2 hover:text-[]">
                        <div class="flex items-center rounded-md hover:bg-[#455259] py-2 px-4 gap-x-2">
                            <i class="fa-solid fa-house-user duration-300 text-white"
                                :class="`${sideToggle == true ? 'ml-[-8px]' : ''}`"></i>
                            <span class="text-[1rem] font-medium duration-300 text-white"
                                :class="`${sideToggle == true ? 'scale-0' : ''}`">Profile</span>
                            <div class="flex-1 text-right duration-300"
                                :class="`${sideToggle == true ? 'scale-0' : ''}`">
                                <i id="icon" class="fa-solid fa-angle-down duration-300 text-white"
                                    :class="`${menuDropDownToggle == true ? 'rotate-180' : ''}`"
                                    @click="menuDropDown()"></i>
                            </div>
                        </div>

                        <div class="pl-5 py-2 duration-300" :class="`${menuDropDownToggle == true ? 'show' : 'hide'}`">
                            <ul>
                                <li>item 01</li>
                                <li>item 01</li>
                                <li>item 01</li>
                                <li>item 01</li>
                            </ul>
                        </div>
                    </li>

                </ul>
            </div>
        </div>


    </div>
</template>

<script>
export default {
    name: "SidebarComponent",
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
.show {
    display: block;
}

.hide {
    display: none;
}
</style>
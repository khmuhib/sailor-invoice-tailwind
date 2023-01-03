<template>
    <div class="flex justify-end items-center gap-x-2">
        <div class="flex gap-x-3">
            <div class="">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                    stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                    class="feather feather-sunrise hover:text-[#00C3FF] text-[#abacad]">
                    <path d="M17 18a5 5 0 0 0-10 0"></path>
                    <line x1="12" y1="2" x2="12" y2="9"></line>
                    <line x1="4.22" y1="10.22" x2="5.64" y2="11.64"></line>
                    <line x1="1" y1="18" x2="3" y2="18"></line>
                    <line x1="21" y1="18" x2="23" y2="18"></line>
                    <line x1="18.36" y1="11.64" x2="19.78" y2="10.22"></line>
                    <line x1="23" y1="22" x2="1" y2="22"></line>
                    <polyline points="8 6 12 2 16 6"></polyline>
                </svg>
            </div>
            <div class="">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                    stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                    class="feather feather-maximize hover:text-[#00C3FF] text-[#abacad]">
                    <path
                        d="M8 3H5a2 2 0 0 0-2 2v3m18 0V5a2 2 0 0 0-2-2h-3m0 18h3a2 2 0 0 0 2-2v-3M3 16v3a2 2 0 0 0 2 2h3">
                    </path>
                </svg>
            </div>
            <div class="">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                    stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                    class="feather feather-globe hover:text-[#00C3FF] text-[#abacad]">
                    <circle cx="12" cy="12" r="10"></circle>
                    <line x1="2" y1="12" x2="22" y2="12"></line>
                    <path
                        d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z">
                    </path>
                </svg>
            </div>
            <div class="relative">
                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none"
                    stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                    class="feather feather-bell hover:text-[#00C3FF] text-[#abacad]">
                    <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                    <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
                </svg>
                <div class="h-[16px] w-[16px] rounded-full bg-[#00C3FF] absolute top-[-7px] right-[-4px]">
                    <span class="text-center block text-[10px] text-white font-bold">2</span>
                </div>
            </div>

        </div>
        <div class="">
            <div class="flex items-center text-right gap-x-2 px-3">
                <div class="">
                    <p class="text-[12px]">Good Morning</p>
                    <p class="text-[14px] font-semibold">Kh Muhib</p>
                </div>
                <div class="">
                    <img class="h-[40px] w-[40px] rounded-full border-2 border-sky-400"
                        src="/src/assets/images/icon01.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "TopbarComponent"

}
</script>

<style>

</style>
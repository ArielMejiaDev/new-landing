<template>
    <nav class="relative z-10 flex items-center justify-between flex-wrap bg-mint lg:bg-transparent p-6 lg:h-40">

        <!-- brand logo -->
        <div class="flex items-center flex-shrink-0 text-pink mr-6">

            <svg class="fill-current h-8 w-8 mr-2" width="54" height="54" viewBox="0 0 54 54" xmlns="http://www.w3.org/2000/svg"><path d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z"/></svg>

            <!-- <img src="" alt=""> -->

            <p class="font-semibold text-3xl tracking-wide text-pink">recaudar.com</p>
        </div>

        <!-- responsive menu -->
        <div class="block lg:hidden">
            <button @click="menuToggle = ! menuToggle" class="flex items-center px-3 py-2 border rounded text-white border-white focus:outline-none">
                <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
                    <title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/>
                </svg>
            </button>
        </div>

        <!-- responsive menu -->
        <transition name="expand">
        <div v-if="menuToggle" class="w-full block flex-grow lg:flex lg:items-center lg:justify-end lg:w-auto">
       
            <div>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-white hover:text-gray-200 text-xl tracking-wide">
                    Quienes somos
                </a>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-white hover:text-gray-200 text-xl tracking-wide">
                    Contacto
                </a>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-pink hover:text-red-600 tracking-wide text-xl uppercase">
                    Covid-19
                </a>

                <a href="#" 
                    class="inline-block text-sm px-6 py-3 lg:mx-2 leading-none border-4 rounded-full text-white lg:text-xl 
                    border-pink bg-transparent hover:bg-pink mt-4 lg:mt-0 tracking-wide">
                    Log in
                </a>
    
                <a href="#" 
                    class="inline-block text-sm px-6 py-3 lg:mx-2 leading-none 
                    border-4 rounded-full text-blue-800 lg:hover:text-white font-bold lg:text-xl 
                    border-mint bg-teal-200 lg:bg-mint lg:hover:bg-transparent mt-4 lg:mt-0 tracking-wider">
                    Crea tu campaña
                </a>

            </div>        

        </div>

        </transition>

        <!-- large menu -->

        <div class="w-full block flex-grow lg:flex lg:items-center lg:justify-end lg:w-auto hidden lg:block">
       
            <div>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-white hover:text-gray-200 text-xl tracking-wide">
                    Quienes somos
                </a>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-white hover:text-gray-200 text-xl tracking-wide">
                    Contacto
                </a>

                <a href="#" class="block mt-4 lg:px-3 lg:inline-block lg:mt-0 text-pink hover:text-red-600 tracking-wide text-xl uppercase">
                    Covid-19
                </a>

                <a href="#" 
                    class="inline-block text-sm px-6 py-3 lg:mx-2 leading-none border-4 rounded-full text-white lg:text-xl 
                    border-pink bg-transparent hover:bg-pink mt-4 lg:mt-0 tracking-wide">
                    Log in
                </a>
    
                <a href="#" 
                    class="inline-block text-sm px-6 py-3 lg:mx-2 leading-none 
                    border-4 rounded-full text-blue-800 lg:hover:text-white font-bold lg:text-xl 
                    border-mint bg-teal-200 lg:bg-mint lg:hover:bg-transparent mt-4 lg:mt-0 tracking-wider">
                    Crea tu campaña
                </a>

            </div>        

        </div>

    </nav>
</template>

<script>
export default {
    name: 'Navbar',
    data: () => {
        return {
            menuToggle: false
        }
    }
}
</script>

<style>
    
    .expand-enter-active, .expand-leave-active {
        transition: all .3s ease-in;
        height: 200px;
        overflow: hidden;
    }

    .expand-enter, .expand-leave-to {
        height: 0;
        opacity: 0;
    }
    

</style>
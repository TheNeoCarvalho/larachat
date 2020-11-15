<template>
    <app-layout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Chat
            </h2>
        </template>

        <div class="py-12">
            <div class="max-w-7xl mx-auto sm:px-6 lg:px-8">
                <div class="bg-white overflow-hidden shadow-xl sm:rounded-lg flex" style="min-height: 400px">
                    <div class="w-3/12 bg-gray-200 shadow-xl bg-opacity-25 border-gray-200">
                        <ul>
                            <li class="p-5 text-lg text-gray-600 leading-7 font-semibold border-b border-gray-200 hover:bg-gray-200 hover:bg-opacity-50 hover:cursor-pointer">
                                <p class="flex items-center">
                                    Manoel
                                    <span class="ml-2 w-2 h-2 bg-blue-200 rounded-full"></span>
                                </p>
                            </li>
                            <li class="p-5 text-lg text-gray-600 leading-7 font-semibold border-b border-gray-200 hover:bg-gray-200 hover:bg-opacity-50 hover:cursor-pointer">
                                <p class="flex items-center">
                                    Manolo
                                    <span class="ml-2 w-2 h-2 bg-blue-200 rounded-full"></span>
                                </p>
                            </li>
                        </ul>
                    </div>
                    <div class="w-9/12">

                        <div class="w-full p-6 flex flex-col">
                            <div class="w-full mb-3 text-right">
                                <p class="inline-block p-2 rounded-md messageFromMe" style="max-width: 75%">
                                    Olá
                                </p>
                                <span class="block mt-1 text-gray-400">21/11/2020 00:24</span>
                            </div>

                            <div class="w-full mb-3 text-left">
                                <p class="inline-block p-2 rounded-md messageToMe" style="max-width: 75%">
                                    Oi
                                </p>
                                <span class="block mt-1 text-gray-400">21/11/2020 00:25</span>
                            </div>
                        </div>
                        <form>
                            <input type="text" name="" >
                            <button>enviar</button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </app-layout>
</template>
+++
<script>
    import AppLayout from '@/Layouts/AppLayout'

    export default {
        components: {
            AppLayout,
        },
    }
</script>
<style>
.messageFromMe {
    @apply bg-indigo-300 bg-opacity-25
}

.messageToMe {
    @apply bg-gray-300 bg-opacity-25
}
</style>

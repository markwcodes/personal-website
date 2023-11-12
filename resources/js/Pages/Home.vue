<script setup>
import { Head } from '@inertiajs/vue3';

defineProps({
    canLogin: Boolean,
    canRegister: Boolean,
    commitShortHash: String,
    appVersion: String,
});
</script>

<template>
    <Head title="Home" />

    <div class="min-h-screen flex items-center justify-center bg-cover bg-center relative" style="background-image: url('https://images.unsplash.com/photo-1587595340454-c1a85f52886d');">
        <!-- Overlay with dark effect -->
        <div class="absolute inset-0 bg-black opacity-75"></div>

        <!-- Main content container -->
        <div class="w-full px-4 sm:px-6 md:px-8 lg:px-10 xl:px-12 relative z-10">
            <div class="max-w-4xl mx-auto bg-white rounded-lg shadow-lg overflow-hidden">
                <!-- Profile header -->
                <div class="text-center p-8 pb-4">
                    <h1 class="text-6xl font-bold mb-4">Mark Wilson</h1>
                    <h2 class="text-4xl">Cloud DevOps Engineer</h2>
                </div>

                <!-- Social links -->
                <div class="flex justify-center space-x-4 mb-4">
                    <!-- LinkedIn Icon -->
                    <a href="https://linkedin.com/in/m2w" target="_blank" class="p-3 relative rounded-full bg-neutral-800 hover:opacity-70 transition-opacity duration-300">
                        <svg class="w-6 h-6 stroke-0" fill="white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
                            <title>Linkedin icon</title>
                            <path d="M7.2 20.8h-4v-12h4v12zM5.202 7.2a2 2 0 11-.004-4 2 2 0 01.004 4zM21.6 20.8h-3.845v-5.84c0-1.393-.027-3.183-2-3.183-2.002 0-2.31 1.516-2.31 3.082V20.8H9.6V8.791h3.69v1.64h.054c.512-.944 1.768-1.939 3.64-1.939 3.896 0 4.616 2.488 4.616 5.722V20.8z"></path>
                        </svg>
                    </a>
                    <!-- GitHub Icon -->
                    <a href="https://github.com/markwcodes" target="_blank" class="p-3 relative rounded-full bg-neutral-800 hover:opacity-70 transition-opacity duration-300">
                        <svg class="w-6 h-6 stroke-0" fill="white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
                            <title>GitHub</title>
                            <path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"></path>
                        </svg>
                    </a>
                    <!-- Email Icon -->
                    <a href="mailto:mark&commat;wilson&period;codes" target="_blank" class="p-3 relative rounded-full bg-neutral-800 hover:opacity-70 transition-opacity duration-300">
                        <svg class="w-6 h-6 stroke-0" fill="white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48">
                            <title>Email</title>
                            <path d="M46.652 1.348L45.432.084 1.302 14.12l-.466 3.484L14.33 28.31 40.746 7.254 19.69 33.67l10.706 13.494 3.484-.466 14.036-44.13-1.264-1.22z"></path>
                        </svg>
                    </a>
                </div>

                <!-- Biography -->
                <div class="px-8 py-4 text-xl leading-8 text-center mb-4">
                    <p>
                        I am a dedicated software development and DevOps professional with over 5 years of full-time experience in high-demand environments. My self-directed education path has not only cultivated a robust skill set but has also ingrained a keen adaptability and an analytical mindset, crucial for solving complex business problems. My colleagues know me as a passionate, supportive and accessible team player, with a zest for IT that started in my youth and has since flourished into a rewarding career.
                    </p>
                </div>

                <!-- Portfolio link -->
                <div class="text-center text-xl pb-8">
                    <a href="https://github.com/markwcodes" target="_blank" class="inline-flex py-2 px-4 rounded text-white font-bold bg-neutral-800 hover:shadow-2xl transition-shadow duration-300">
                        <svg class="w-6 pr-1.5 stroke-0" fill="white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 30 30">
                            <title>Link</title>
                            <path d="M9.631 3.225l12.033 12.032L21 17l-5.56.04 3.573 7.915a1.438 1.438 0 11-2.63 1.163L12.92 18.12l-3.177 3.545L8 21V4l1.631-.775z"></path><path d="M9 3a1 1 0 100 2 1 1 0 100-2zm0 17a1 1 0 100 2 1 1 0 100-2zm12-5a1 1 0 100 2 1 1 0 100-2z"></path>
                        </svg>
                        My portfolio
                    </a>
                </div>
            </div>
        </div>
    </div>

    <div class="p-2 bg-black text-white fixed bottom-0 left-0 w-full inline-flex justify-center">
        This site and its&nbsp;<a href="https://github.com/markwcodes/personal-website-infra" target="_blank">DevOps infrastructure</a>&nbsp;are open source!
        <a href="https://github.com/markwcodes/personal-website" target="_blank" class="inline-flex">
            <svg class="h-6 ml-2" fill="white" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
                <path d="M15 12C15 13.6569 13.6569 15 12 15C10.3431 15 9 13.6569 9 12M15 12C15 10.3431 13.6569 9 12 9C10.3431 9 9 10.3431 9 12M15 12H21M9 12H3" stroke="#FFFFFF" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
            {{ commitShortHash }} - (v{{ appVersion }})
        </a>
    </div>
</template>

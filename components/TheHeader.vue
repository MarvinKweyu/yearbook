<template>
    <div>
        <h1 class="text-center text-6xl font-bold">The Yearbook</h1>
        <p class="text-center text-xl font-semibold">The best yearbook ever</p>
        <div class="flex justify-center">
            <router-link to="/us" class="mx-2 cursor-pointer">Us</router-link>
            <router-link to="/fun-times" class="mx-2 cursor-pointer">Fun Times</router-link>
            <router-link to="/" class="mx-2 cursor-pointer">Staff</router-link>
        </div>
        <div class="flex justify-center">
            <div class="my-3">
                <input type="search"
                    class="relative m-0 text-center block w-full min-w-0 flex-auto rounded border border-solid border-neutral-300 bg-transparent bg-clip-padding px-3 py-[0.25rem] text-base font-normal leading-[1.6] text-neutral-700 outline-none transition duration-200 ease-in-out focus:z-[3] focus:border-primary focus:text-neutral-700 focus:shadow-[inset_0_0_0_1px_rgb(59,113,202)] focus:outline-none dark:border-neutral-600 dark:text-neutral-200 dark:placeholder:text-neutral-200 dark:focus:border-primary"
                    id="search" placeholder="Search..." />
            </div>
        </div>

    </div>
</template>
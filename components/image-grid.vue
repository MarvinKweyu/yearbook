<template>

    <div class="grid grid-cols-6 gap-4 mx-6 mt-4">
        <img v-for="img in 10" :key="img" src="https://picsum.photos/400" alt="" class="rounded cursor-pointer">
    </div>
</template>
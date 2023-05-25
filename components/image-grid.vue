<template>
    <div class="grid grid-cols-1 md:grid-cols-6 gap-4 mx-6 mt-4">
        <div v-for="img in 10" :key="img" class="cursor-pointer mt-2">
            <img src="https://picsum.photos/500" alt="" class="rounded-t-md">
            <div class="bg-amber-200 text-sm h-24 rounded-b-md">
                <p class="text-center font-medium text-lg">Random name</p>
                <p class="text-center text-md">Kenya</p>
                <div class="flex justify-center items-center ">
                    <p class="text-center text-xs">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.
                    </p>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
/* (A) RESPONSIVE IMAGE */
.fullwrap img {
    width: 100%;
}

.fullwrap {
    max-width: 500px;
    /* optional */
    position: relative;
    /* required for (b1) */
}

/* (B) POSITION CAPTION */
.fullcap {
    /* (B1) COVER OVER ENTIRE IMAGE */
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.3);

    /* (B2) CENTER CONTENT */
    display: flex;
    justify-content: center;
    align-items: center;
}

/* (C) ONLY SHOW CAPTION ON HOVER */
.fullcap {
    visibility: none;
    opacity: 0;
    transition: opacity 0.3s;
}

.fullwrap:hover .fullcap {
    visibility: visible;
    opacity: 1;
}
</style>
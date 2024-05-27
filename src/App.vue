<script>
import { ref } from 'vue';

export default {
    setup() {
        const username = ref("");
        const password = ref("");
        const email = ref("")
        
        return { username, password, email };
    }
}
</script>
<template>
    <div>
        <p class="p-4">username: {{ username }}</p>
        <p class="p-4">email: {{ email }}</p>
        <p class="p-4">password: {{ password }}</p>
    </div>
    <div class="  flex flex-col  items-center ">
        <form class=" flex flex-col items-center  bg-yellow-300 rounded-2xl h-auto w-1/2 p-5 ">
            <div class=" flex flex-col w-80  p-2">
                <label class="   ">username</label>
                <input class="rounded-lg h-10   " v-model="username" type="text" placeholder="username" />
            </div>
            <div class="flex flex-col w-80 p-2">
                <label>email</label>
                <input class="rounded-lg h-10 " v-model="email" type="email" placeholder="email" />
            </div>
            <div class=" flex flex-col w-80 p-2">
                <label>password</label>
                <input class="rounded-lg mb-4 h-10 " v-model="password" type="password" placeholder="password" />
            </div>
            <div class=" w-80  flex-row items-center">
                <label class=" ml-3"><input type="checkbox" /></label>
                pps
            </div>
        </form>
    </div>
</template>

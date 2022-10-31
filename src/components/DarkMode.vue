<template>
    <div>
        <button @click="toggle" class="cursor-pointer absolute top-10 dark:bg-white dark:text-black text-white bg-black rounded p-4">{{ name }}</button>
    </div>
</template>

<script>
export default {
    name: "DarkMode",
    data(){
        return {
            isDark: false,
        }
    },  
    computed: {
        name() {
            return this.isDark ? 'Light' : 'Dark'
        }
    },
    watch: {
        isDark(vl){
            const html = document.querySelector("html");
            if(vl){
                html.classList.add("dark")
            } else {
                html.classList.remove("dark")
            }
        }
    },

    methods: {
        toggle(){
            this.isDark = !this.isDark
        }
    }
}
</script>
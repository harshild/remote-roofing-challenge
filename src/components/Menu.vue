<template>
    <div>
        <div v-for="(value, name) in items" :key="value" >
            <a :href="value">{{ name }}</a>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Menu",
        data() {
            return {
            items: {
                Home: "https://www.remoteroofing.com/",
                FAQ: "https://www.remoteroofing.com/faq",
                Services: "https://www.remoteroofing.com/#services"
            }
        }
    },

    }
</script>

<style scoped>

</style>

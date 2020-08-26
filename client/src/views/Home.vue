<template>
    <div class="home">
        <img alt="Vue logo" src="../assets/logo.png" />
        <HelloWorld msg="Welcome to Your Vue.js App" />
    </div>
</template>

<style scoped>
.home {
    background-color: #fff;
}
</style>

<script>
// @ is an alias to /src
export default {
    name: "Home",
    components: {
        HelloWorld: () =>
            import(
                /* webpackChunkName: "helloworld" */ "@/components/HelloWorld.vue"
            ),
    },
};
</script>

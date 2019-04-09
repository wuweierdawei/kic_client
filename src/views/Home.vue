<template>
    <div class="home">
        <img alt="Vue logo" src="../assets/logo.png">
        <HelloWorld v-bind:msg="first+name"></HelloWorld>
    </div>
</template>

<script>
    // @ is an alias to /src
    import HelloWorld from '@/components/HelloWorld.vue';

    let first = function () {
        return {
            first: "li"
        }
    };
    export default {
        name: 'home',
        components: {
            HelloWorld
        },
        data: first,
        computed:
            {
                name: function () {
                    return "dawei"
                }
            }
    }
</script>

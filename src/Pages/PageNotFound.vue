<template>
    <div class="col-full" :class="$style.centered">
        <h1 :class="$style['heading-large']">Not Found</h1>
        <p :class="$style['text-large']">No page here</p>
        <router-link :to="{ name: 'Home'}" >
            Go home instead?
        </router-link>
    </div>
</template>

<script>
    export default {
        created () {
            this.$emit('ready')
        }
    }
</script>

<style module>
    .heading-large {
        font-size: 100px;
    }
    .text-large {
        font-size: 50px;
        font-weight: 100;
    }
    .centered {
        text-align: center;
    }
</style>
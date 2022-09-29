<template>
    <div>
        <Theheader />
        <nuxt/>
        <Thefooter />

    </div>
</template>

<script>
import Theheader from '../components/Theheader.vue';
import Thefooter from '../components/Thefooter.vue';
export default {
    components: { Theheader, Thefooter }
}
</script>

<style lang="scss">

</style>
<template>
    <main>
        <GetStartTop/>
        <Businesses/>
    </main>
</template>

<script>
import GetStartTop from '../sections/GetStartTop.vue';
import Businesses from '../sections/Businesses.vue';

export default {
    name: 'Main',
    components: {
        GetStartTop,
        Businesses
    }
}
</script>

<style lang='scss' scoped>

</style>
<template>
    <main>
        <GetStartTop/>
        <Businesses/>
        <Deploy/>
    </main>
</template>

<script>
import GetStartTop from '../sections/GetStartTop.vue';
import Businesses from '../sections/Businesses.vue';
import Deploy from '../sections/Deploy.vue';

export default {
    name: 'Main',
    components: {
        GetStartTop,
        Businesses,
        Deploy
    }
}
</script>

<style lang='scss' scoped>

</style>
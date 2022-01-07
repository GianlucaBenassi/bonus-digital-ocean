<template>
    <main>
        <GetStartTop/>
        <Businesses/>
        <Deploy/>
        <Designe/>
    </main>
</template>

<script>
import GetStartTop from '../sections/GetStartTop.vue';
import Businesses from '../sections/Businesses.vue';
import Deploy from '../sections/Deploy.vue';
import Designe from '../sections/Designe.vue';

export default {
    name: 'Main',
    components: {
        GetStartTop,
        Businesses,
        Deploy,
        Designe
    }
}
</script>

<style lang='scss' scoped>

</style>
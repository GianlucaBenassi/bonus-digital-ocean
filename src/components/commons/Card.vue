<template>
    <div>
        <img :src="infos.img" :alt="infos.title">
        <h4 class="fw-bold mt-2">{{infos.title}}</h4>
        <p>{{infos.desc}}</p>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        infos: Object
    }
}
</script>

<style lang='scss' scoped>

@import '../../assets/style/variables.scss';

p {
    color: $textColor;
}

</style>
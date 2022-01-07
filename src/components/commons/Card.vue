<template>
    <div>
        <img :src="infos.img" :alt="infos.title">
        <h4 class="fw-bold mt-2">{{infos.title}}</h4>
        <p>{{infos.desc}}</p>
        <a href="#" v-if="infos.link">{{infos.link}} &gt;</a>
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

a {
    color: $mainColor;

    &:hover {
        text-decoration: underline;
    }
}

</style>
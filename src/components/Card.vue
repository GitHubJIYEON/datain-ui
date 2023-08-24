<template>
    <div class="card-component">
        <h4 class="title">{{ title }}</h4>
        <p class="desc">
            {{ desc }}
        </p>
        <a href="#" type="button" class="btn btn-round btn-full btn-black">
            <b>+</b> 시작하기
        </a>
    </div>
</template>
<script setup>
const props = defineProps({
    title: String,
    desc: String,
});

</script>
<style lang="scss" scoped>
.card-component {
    border: 1px solid var(--border-color2);
    background-color: var(--bg-color);
    box-shadow: var(--shadow-1);
    border-radius: 2.4rem;
    padding: 6rem 4rem;
    font-size: 1.6rem;

    > .title {
        font-size: 2.4rem;
        font-weight: 500;
    }

    > .desc {
        margin-top: 2.1rem;
        line-height: 150%;
    }

    > .btn {
        margin-top: 7.5rem;
    }
}
</style>

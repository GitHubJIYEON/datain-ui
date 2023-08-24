<template>
    <div class="card-component">
        <a href="#">
            <h4 class="title">{{ title }}</h4>
            <div class="img-box">
                <img :src="props.imgSrc" :alt="title" />
            </div>
        </a>
    </div>
</template>
<script setup>
const props = defineProps({
    title: String,
    imgSrc: String,
});
</script>
<style lang="scss" scoped>
.card-component {
    border: 1px solid var(--border-color2);
    background-color: var(--bg-color);
    box-shadow: var(--shadow-1);
    border-radius: 0.8rem;
    padding: 4rem 0;
    font-size: 1.6rem;

    .title {
        font-size: 3.2rem;
        text-align: center;
        font-weight: 300;
        line-height: 1.4;
    }

    .img-box {
        width: 16.3rem;
        height: 7.4rem;
        margin: 2.4rem auto 0;
        position: relative;

        > img {
            // margin-right: 3.2rem;
        }

        &::after {
            content: "\2b";
            text-align: center;
            line-height: 2.8rem;
            display: block;
            position: absolute;
            top: 50%;
            right: 0;
            transform: translateY(-50%);
            width: 2.4rem;
            height: 2.4rem;
            border-radius: 50%;
            background-color: var(--font-color);
            color: var(--font-color2);
            filter: drop-shadow(0px 6px 8px rgba(0, 0, 0, 0.1));
        }
    }
}
</style>

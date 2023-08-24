<template>
    <LeftMenu />
    <div class="container container-type2">
        <TopTitle />
        <div class="card-group">
            <Card title="객관식 유형" imgSrc="../src/assets/img/sub/q_type1.png"/>
            <Card title="입력식 유형" imgSrc="../src/assets/img/sub/q_type2.png"/>
            <Card title="척도형 유형" imgSrc="../src/assets/img/sub/q_type3.png"/>
            <Card title="설명형 유형" imgSrc="../src/assets/img/sub/q_type4.png"/>
        </div>
        <p class="sub-info-text">
            설문유형을 선택하여 주세요!
        </p>
    </div>
    <RightMenu/>
</template>
<script setup>
import Card from "@/components/Card2.vue";
import LeftMenu from "@/components/common/LeftMenu.vue";
import TopTitle from "@/components/common/TopTitle.vue";
import RightMenu from "@/components/common/RightMenu.vue";
</script>
<style lang="scss">
.container{
    padding-top: 7.3rem;
}

.card-group {
    display: flex;
    flex-wrap: wrap;
    width: 58.6rem;
    justify-content: space-around;
    margin: 16rem auto 0;
    gap: 1rem .5rem;
    
    > .card-component {
        width: calc(50% - 1rem);
        height: 24.4rem;
    }
}

.sub-info-text {
    padding: 2rem;
    text-align: center;
    line-height: 1.7;
    font-size: 1.4rem;
}
</style>

<template>
    <div class="survey-page container">
        <h3 class="page-title">신규 설문 등록</h3>
        <div class="card-wrap">
            <Card
                title="새로운 설문 작성하기 👋🏻"
                desc="설문조사와 분석보고서,\n
    논문통계보고서까지 자동으로\n
    완성합니다."
    link = "/write"
            />
            <Card
                title="템플릿 활용하기! 👌"
                desc="데이터만 입력하세요\n
    템플릿 활용으로\n
    보고서를 자동으로 완성합니다"
            />
        </div>
    </div>
</template>
<script setup>
import Card from "@/components/Card.vue";
import Footer from "@/components/common/Footer.vue";
</script>
<style lang="scss" scoped>
    .survey-page {
        .card-wrap {
            display: flex;
            width: 74.4rem;
            justify-content: space-between;
            gap: 2.4rem;
            margin: auto;

            .card-component {
                width: 50%;
            }
        }
    }
</style>

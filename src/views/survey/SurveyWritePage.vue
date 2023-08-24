<template>
    <div class="survey-page container">
        <h3 class="page-title">새로운 설문 작성하기 👋🏻</h3>
        <Step />
        <form action="">
            <FormGroup></FormGroup>
        </form>
        <div class="bottom-btn-row">
            <a href="#" class="btn-move prev text">이전</a>
            <a href="#" class="btn-move next text">다음</a>
            <!-- <button href="#" class="btn-move next text">다음</button> -->
        </div>
        <div class="bottom-btn-row">
            <button type="button" class="btn btn-round btn-full">
                <i class="fa-solid fa-check"></i> 작성완료
            </button>
        </div>
    </div>
</template>
<script setup>
import FormGroup from "@/components/FormGroup.vue";
import Step from "@/components/Step.vue";
</script>
<style lang="scss" scoped>
.survey-page {
    &.container {
        width: 98rem;
    }

    .step-component {
        width: calc(100% - 31rem);
    }

    .form-group-component {
        &:first-child {
            margin-top: 3rem;
        }
        margin-top: 1.3rem;
    }

    .bottom-btn-row {
        margin-top: 1rem;
        text-align: right;

        .btn-move {
            margin-left: 2.4rem;

            &:first-child {
                margin-left: 0;
            }
        }

        .btn-full {
            width: 25.2rem;
            margin: 0 auto;
            display: block;
        }
    }
}
</style>

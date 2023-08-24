<template>
    <div class="col col-3">
        <div class="tit">1. Card</div>
        <div class="cont">
            <Card
                title="템플릿 활용하기! 👌"
                desc="데이터만 입력하세요\n
    템플릿 활용으로\n
    보고서를 자동으로 완성합니다"
            />
        </div>
    </div>
    <div class="col col-3">
        <div class="tit">2. Step</div>
        <div class="cont">
            <Step />
        </div>
    </div>
    <div class="col col-3">
        <div class="tit">3. FormGroup</div>
        <div class="cont">
            <!-- <FormGroup /> -->
            등록 부분 참고
        </div>
    </div>
    <div class="col col-3">
        <div class="tit">4. 말줄임 - 1줄, 2줄</div>
        <div class="cont">
            <p class="text-ellipsis">
                해당 클래스를 사용하면 1줄 넘어가면 말줄임표 처리가 됩니다 1줄 넘어가면 말줄임표 처리가 됩니다 1줄 넘어가면 말줄임표 처리가 됩니다 1줄 넘어가면 말줄임표 처리가 됩니다 
            </p>
            <hr>
            <p class="text-ellipsis-line2">
                해당 클래스를 사용하면 2줄 넘어가면 말줄임표 처리가 됩니다 2줄 넘어가면 말줄임표 처리가 됩니다 2줄 넘어가면 말줄임표 처리가 됩니다 2줄 넘어가면 말줄임표 처리가 됩니다 
            </p>
        </div>
    </div>
</template>
<script setup>
import Card from "@/components/Card.vue";
import FormGroup from "@/components/FormGroup.vue";
import Step from "@/components/Step.vue";
</script>

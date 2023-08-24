<template>
    <!-- <div class="step-component">
        <div class="step current">
            <i class="step-icon">1</i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 01</small>
                설문-기본정보 설정하기
            </h4>
        </div>
        <div class="step">
            <i class="step-icon">2</i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 02</small>
                설문-옵션 설정하기
            </h4>
        </div>
        <div class="step">
            <i class="step-icon">3</i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 03</small>
                설문-기본스타일 설정하기
            </h4>
        </div>
        <div class="step">
            <i class="step-icon">4</i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 04</small>
                설문-안내문/마무리말 설정하기
            </h4>
        </div>
    </div> -->
    <!-- toptitle component step -->
    <div class="step-component">
        <div class="step current">
            <i class="step-icon"><i class="fa-solid fa-laptop"></i></i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 01</small>
                작성중
            </h4>
        </div>
        <div class="step">
            <i class="step-icon"><i class="fa-solid fa-play"></i></i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 02</small>
                진행중
            </h4>
        </div>
        <div class="step">
            <i class="step-icon"><i class="fa-solid fa-stop"></i></i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 03</small>
                중지
            </h4>
        </div>
        <div class="step">
            <i class="step-icon"><i class="fa-solid fa-check"></i></i>
            <h4 class="tit">
                <small class="sub-tit">STEP. 04</small>
                종료
            </h4>
        </div>
    </div>
</template>
<script setup></script>
<style lang="scss" scoped>
.step-component {
    display: flex;
    justify-content: space-between;
    position: relative;
    margin: 0 auto;
    padding-bottom: 5.2rem;
    user-select: none;

    .step {
        text-align: center;
        position: relative;

        &:first-child {
            margin-left: 5rem;
        }

        &:last-child {
            margin-right: 5rem;
        }

        &.current {
            .step-icon {
                background-color: var(--primary-color);
                font-size: 0;

                &:after {
                    font-family: var(--icon-font);
                    content: "\f00c";
                    color: var(--bg-color);
                    font-size: 1.8rem;
                    display: inline-block;
                    margin-top: -0.2rem;
                }
            }
            .tit {
                opacity: 100%;
                color: var(--primary-color);
            }
        }

        &-icon {
            display: block;
            width: 4.8rem;
            height: 4.8rem;
            border-radius: 50%;
            background-color: var(--border-color2);
            text-align: center;
            color: var(--font-color3);
            line-height: 5.4rem;
            font-size: 2rem;
            position: relative;
            margin: auto;
        }

        .sub-tit {
            display: block;
            margin-top: 1rem;
            font-size: 1.4rem;
            line-height: 1.71;
            color: var(--font-color);
        }
        .tit {
            font-size: 1.6rem;
            opacity: 0;
            color: var(--font-color3);
            font-weight: 400;
            line-height: 1.5;
            position: absolute;
            width: max-content;
            left: 50%;
            transform: translateX(-50%);
        }
    }

    &::after {
        content: "";
        display: block;
        position: absolute;
        top: 2.6rem;
        width: calc(100% - 11rem);
        left: 5.5rem;
        z-index: -1;
        border: 1px dotted var(--border-color2);
    }
}
</style>

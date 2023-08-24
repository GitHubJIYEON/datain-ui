<template>
    <nav class="top-title">
        <h3 class="title">학부모 교육 만족도 조사</h3>
        <button type="button" class="btn-icon type2">
            <i class="fa-solid fa-star icon"></i>즐겨찾기
        </button>
        <button type="button" class="btn-icon type2">
            <i class="fa-solid fa-pen-nib icon"></i>수정
        </button>
        <div class="step-r">
            <Step />
        </div>
    </nav>
</template>
<script setup>
import Step from "../Step.vue";
</script>
<style lang="scss">
.top-title {
    position: fixed;
    top: 6.6rem;
    height: 7.3rem;
    display: flex;
    align-items: center;
    padding: 0 30rem;
    border-bottom: .3rem solid var(--bg-color2);
    background-color: var(--bg-color);
    width: calc(100%);
    left: 0;

    .title {
        display: inline-block;
        line-height: 1.3;
        vertical-align: middle;
        padding-left: 6rem;
    }

    .btn-icon {
        vertical-align: middle;
        line-height: 1rem;
        margin-top: 0.2rem;
        margin-left: 0.2rem;
        color: var(--border-color3);

        > i {
            font-size: 1.4rem;
        }
    }

    > .step-r {
        width: 22.8rem;
        margin-left: auto;
        margin-right: 17.8rem;

        > .step-component {
            padding: 0;
            margin-top: -1.5rem;

            &::after {
                width: calc(100% - 1rem);
                left: 0;
                top: 50%;
            }
            .step {
                &-icon {
                    width: 2.5rem;
                    height: 2.5rem;
                    font-size: 0.9rem;
                    line-height: 2.5rem;
                    border: 1px solid var(--border-color2);
                    background-color: var(--btn-gray);
                }

                &.current .step-icon {
                    font-size: 0.9rem;
                    color: var(--bg-color);
                    &::after {
                        display: none;
                    }
                }

                &:first-child,
                &:last-child {
                    margin: 0;
                }
            }

            .tit {
                font-size: 1.3rem;
                opacity: 100%;
                line-height: 1.5;
                margin-top: 0.4rem;
            }
            .sub-tit {
                display: none;
            }
        }
    }
}
</style>

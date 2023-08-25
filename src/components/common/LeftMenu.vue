<template>
    <aside class="left-menu" :class="{ open: isActive }">
        <div class="y-scroll">
            <button type="button" class="btn-menu-fold" @click="leftsideToggle">열고접기</button>
            <button type="button" class="btn btn-gray btn-full btn-align-l">
                <i class="icon">👋🏻 </i>신규 설문 등록
            </button>
            <h4 class="left-menu-tit">
                설문 프로젝트 <span class="tit-label">총 13개</span>
                <button class="btn-text">전체보기</button>
            </h4>
            <section class="left-menu-select">
                <select name="selc" id="selc" class="text-ellipsis">
                    <option value="">
                        프로젝트 명 프로젝트 명 프로젝트 명 프로젝트 명
                    </option>
                    <option value="1">1번</option>
                    <option value="2">2번</option>
                    <option value="3">3번</option>
                </select>
            </section>
            <h4 class="left-menu-tit">
                설문 문항 <span class="tit-label">총 54문항</span>
                <button class="btn-icon type2" type="button">
                    <i class="fa-solid fa-magnifying-glass icon"></i>
                    검색
                </button>
                <button class="btn-text">문항 바로가기</button>
            </h4>
            <section class="left-card-list">
                <div class="list-top">
                    <input type="checkbox" name="ch" id="ch" class="check-s" />
                    <label for="ch">선택</label>
                    <button type="button" class="btn-icon type2">
                        <i class="fa-solid fa-ellipsis icon"></i>더보기
                    </button>
                </div>
                <ul class="card-list">
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q1 <span class="small-txt">(단일응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ1) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card disabled">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card active">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q3 <span class="small-txt">(다중응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            조사지 작성 전 학교급식 정보를 확인하여 주시기
                            바랍니다.
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 DQ2) 응답자 설명 
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                    <li class="card">
                        <p class="tit">
                            <input
                                type="checkbox"
                                name="ch"
                                id="ch"
                                class="check-s"
                            />
                            <label for="ch" class="hide">선택</label>
                            Q2 <span class="small-txt">(순위응답)</span>
                        </p>
                        <div class="desc text-ellipsis-line2">
                            DQ2) 응답자 설명
                        </div>
                        <button class="btn-icon type2" type="button">
                            <i class="fa-solid fa-square-plus icon"></i>문항추가
                        </button>
                    </li>
                </ul>
            </section>
            <section class="bottom-btn">
                <button type="button" class="btn btn-white btn-full btn-align-l">
                    <i class="icon">👌 </i>문항 라이브러리 사용하기
                </button>
            </section>
        </div>
    </aside>
</template>
<script setup>
import { ref } from 'vue'

const isActive = ref(true)

const leftsideToggle = () => {
    isActive.value = !isActive.value    
}
</script>
<style lang="scss" scoped>
.left-menu {
    display: inline-block;
    padding: 0 2.4rem;
    width: 30rem;
    height: calc(100vh - 6.6rem);
    border-right: 1px solid var(--border-color2);
    padding-right: 0;
    transition: transform 0.4s ease;
    transform: translateX(-30rem);
    position: absolute;
    background-color: var(--bg-color);
    z-index: 9;
    top: 6.6rem;
    
    &.open {
        transform: translateX(0);
        .btn-menu-fold::after {
            content: "\f053";
        }
    }

    .y-scroll {
        padding: 2rem 2.4rem 0 0;
    }
    .btn-menu-fold {
        position: absolute;
        width: 1.4rem;
        height: 3.8rem;
        border: 1px solid var(--border-color2);
        border-left: 0;
        font-size: 0;
        border-radius: 0 0.3rem 0.3rem 0;
        right: -1.4rem;
        z-index: 99;
        top: 50%;
        transform: translateY(-50%);

        &::after {
            content: "\f054";
            font-size: 1.2rem;
            font-family: var(--icon-font);
            margin-left: -0.2rem;
        }
    }

    &-tit {
        margin: 2rem 0 0.4rem;
        height: 2.4rem;
        display: flex;
        align-items: center;
        font-weight: 400;
        font-size: 1.4rem;

        > .tit-label {
            font-size: 1.2rem;
            color: var(--font-color3);
            display: block;
            line-height: 1.3;
            padding: 0.2rem 0.7rem 0;
            border-radius: 1rem;
            background-color: #ddd;
            margin: 0 0.4rem;
        }

        .btn {
            &-text {
                margin-left: auto;
                font-size: 1.3rem;
                color: var(--font-color3);

                &:hover {
                    text-decoration: underline;
                    color: var(--font-color-link);
                }
            }
        }
    }

    &-select {
        & > select {
            width: 100%;
            background-color: var(--btn-gray);
            color: var(--primary-color);
            font-size: 1.4rem;
        }
    }

    .left-card-list {
        font-size: 1.3rem;
        padding-bottom: 10.5rem;

        > .list-top {
            height: 3.6rem;
            display: flex;
            align-items: center;
            > .btn-icon {
                margin-left: auto;
            }
        }

        .card-list {
            // overflow-y: auto;
            // height: calc(100vh - 6.6rem - 31rem);
            > .card {
                padding: 1.4rem;
                border: 1px solid var(--border-color2);
                border-radius: 0.8rem;
                margin-top: 2.4rem;
                transition: all 0.3s ease-out;
                position: relative;

                &:first-child {
                    margin-top: 0;
                }
                &:hover {
                    border-color: var(--font-color-link);
                }
                &.active {
                    border-color: var(--font-color-link);
                    background-color: #3f8cff08;

                    > .tit {
                        color: var(--font-color-link);

                        .small-txt {
                            color: var(--font-color);
                        }
                    }

                    > .desc {
                        color: var(--font-color-link);
                    }
                }

                > .tit {
                    height: 2.6rem;
                    line-height: 2.6rem;

                    .check-s {
                        margin-right: 0.4rem;
                    }

                    .small-txt {
                        color: var(--font-color3);
                        font-size: 1.2rem;
                    }
                }

                > .desc {
                    margin-top: 0.4rem;
                    line-height: 1.5;
                }

                > .btn-icon {
                    position: absolute;
                    left: 50%;
                    bottom: -2.5rem;
                    font-size: 1.3rem;
                    transform: translateX(-50%);
                }
            }
        }
    }

    .bottom-btn {
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(calc(-50% - 1rem));
        width: calc(100% - 1.1rem);
        padding: 2rem 3rem 4rem;
        background-color: var(--bg-color);
        z-index: 99;

        > .btn-white {
            color: var(--font-color);
        }
    }
}
</style>

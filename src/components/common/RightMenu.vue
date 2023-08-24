<template>
    <aside class="right-menu open">
        <div class="y-scroll">
            <button type="button" class="btn-menu-fold">크게보기</button>
            <button type="button" class="btn-menu-expand">
                <i
                    class="icon fa-solid fa-up-right-and-down-left-from-center"
                ></i>
                열고접기
            </button>
            <section class="sec-line sec-text">
                <h4 class="right-menu-tit">설문유형</h4>
                <p class="text-wrap">
                    1. 객관식<br />
                    정해진 선택지 안에서 응답을 고르는 문항입니다<br /><br />
                    2. 입력형<br />
                    응답자가 숫자와 문자를 직접 입력하는 문항입니다 <br /><br />
                    3. 척도형<br />
                    표 형식 및 의미분화 척도 양식을 제공하는 문항입니다. (모바일
                    환경에서는 일반 문항 양식으로 표기됩니다.) <br /><br />
                    4. 설명형<br />
                    설문에 필요한 설명문을 작성하는 문항입니다.<br />
                    응답을 받지 않는 문항입니다.
                </p>
            </section>
            <section class="sec-line sec-form">
                <h4 class="right-menu-tit">
                    문항 옵션<i class="fa-solid fa-circle-info tooltip"
                        ><span class="tooltip-desc"
                            >설문응답에 관련된 로그인 필요한</span
                        ></i
                    >
                </h4>
                <div class="row">
                    <input
                        type="checkbox"
                        name="ch"
                        id="ch"
                        class="check-s"
                        checked
                    />
                    <label for="ch">필수문항</label>
                </div>
                <div class="row">
                    <input type="checkbox" name="ch" id="ch1" class="check-s" />
                    <label for="ch1">보기 무작위 정렬</label>
                </div>
                <div class="row">
                    <input type="checkbox" name="ch" id="ch2" class="check-s" />
                    <label for="ch2">기타 문항 추가</label>
                </div>
                <div class="row">
                    <input type="checkbox" name="ch" id="ch3" class="check-s" />
                    <label for="ch3">없음 추가</label>
                </div>
                <div class="row">
                    <input type="checkbox" name="ch" id="ch4" class="check-s" />
                    <label for="ch4">자동보기 번호</label>
                </div>
                <div class="row">
                    <input type="checkbox" name="ch" id="ch5" class="check-s" />
                    <label for="ch5">필수 순위 체크</label>
                </div>

                <div class="row">
                    <div class="tit">보기 정렬</div>
                    <div class="desc">
                        <select name="sele" id="sele" class="select-s">
                            <option value="sele">200</option>
                            <option value="sele">200</option>
                            <option value="sele">200</option>
                        </select>
                    </div>
                </div>

                <div class="row">
                    <div class="tit">보기 추가</div>
                    <div class="desc">
                        <select name="sele" id="sele2" class="select-s">
                            <option value="sele2">1</option>
                            <option value="sele2">1</option>
                            <option value="sele2">1</option>
                        </select>
                    </div>
                </div>

                <div class="row row-wide">
                    <span class="txt-b">최소</span>
                    <select name="sele" id="sele2" class="select-s">
                        <option value="sele2">선택</option>
                        <option value="sele2">1</option>
                        <option value="sele2">1</option>
                    </select>
                    <span class="txt">개 에서</span>
                    <select name="sele" id="sele2" class="select-s">
                        <option value="sele2">선택</option>
                        <option value="sele2">1</option>
                        <option value="sele2">1</option>
                    </select>
                    <span class="txt">개 까지</span>
                    <span class="txt-b">응답을 허용합니다</span>
                </div>
            </section>
            <section class="sec-line sec-form">
                <h4 class="right-menu-tit">
                    보기 한번에 붙여 넣기
                    <button type="button" class="btn-white btn-open">
                        <i class="fa-solid fa-door-open"></i> OPEN
                    </button>
                    <button type="button" class="btn-icon type2">
                        <i class="fa-solid fa-caret-down icon"></i> 더보기
                    </button>
                </h4>
                <div class="clipboard-group">
                    <input type="checkbox" name="ch" id="ch" class="check-s" />
                    <label for="ch"
                        >글머리 숫자제거('1)','(1)','[1]',"①",'1.','1 '),
                        <br />특수문자제거 (𝟌,◯)</label
                    >
                    <textarea />
                    <div class="btn-wrap">
                        <button type="button" class="btn btn-black btn-right">
                            붙여넣기
                        </button>
                    </div>
                </div>
            </section>
            <section class="sec-line">
                <h4 class="right-menu-tit">
                    표본및 할당 설정
                    <button type="button" class="btn btn-black btn-right">
                        설정하기
                    </button>
                </h4>
            </section>
            <section class="sec-line">
                <h4 class="right-menu-tit">
                    설문 링크
                    <button type="button" class="btn-icon type2 btn-right">
                        <i class="fa-solid fa-caret-up icon"></i> 더보기
                    </button>
                </h4>
                <div class="tab-group">
                    <div class="tab-group-btn">
                        <button type="button" class="active">
                            설문링크(일반)
                        </button>
                        <button type="button">
                            설문링크(개인별)
                        </button>
                    </div>
                    <div class="tab-group-content">
                        <div class="tab-content">
                            <a
                                class="link-text"
                                href="http://datain.co.kr/reply/survey.html?idx=3964"
                                >http://datain.co.kr/reply/survey.html?idx=xxx</a
                            >
                            <div class="qrcode-group">
                                <div class="code-imgbox">
                                    <img src='http://datain.co.kr/survey/qrcode.html?idx=3964'>
                                </div>
                                <p class="desc">
                                    큐알코드 사용법<br />
                                    1. 이미지 저장 후 파일첨부를 이용하여 전달<br />
                                    2. HTML 작성 시 큐알코드 URL 이용<br />
                                </p>
                            </div>
                        </div>
                        <div class="tab-content"></div>
                    </div>
                </div>
            </section>
            <section class="sec-line">
                <h4 class="right-menu-tit">
                    설문 프로젝트 정보 수정
                    <button type="button" class="btn btn-white btn-right">
                        수정하기
                    </button>
                </h4>
            </section>
        </div>
    </aside>
</template>
<script setup></script>
<style lang="scss" scoped>
.right-menu {
    display: inline-block;
    width: 30rem;
    height: calc(100vh - 6.6rem);
    border-left: 1px solid var(--border-color2);
    transition: transform 0.4s ease;
    transform: translateX(30rem);
    position: absolute;
    background-color: var(--bg-color);
    z-index: 9;
    right: 0;
    top: 6.6rem;

    &.open {
        transform: translateX(0);
        .btn-menu-fold::after {
            content: "\f054";
        }
    }

    .btn {
        &-menu-fold {
            position: absolute;
            width: 1.4rem;
            height: 3.8rem;
            border: 1px solid var(--border-color2);
            border-right: 0;
            font-size: 0;
            border-radius: 0.3rem 0 0 0.3rem;
            left: -1.4rem;
            z-index: 99;
            top: 50%;
            transform: translateY(-50%);

            &::after {
                content: "\f053";
                font-size: 1.2rem;
                font-family: var(--icon-font);
                margin-left: -0.2rem;
            }
        }
        &-menu-expand {
            font-size: 0;
            color: var(--font-color3);
            border: 0;
            margin: 0.7rem 0 0 0.5rem;
            > .icon {
                font-size: 1.3rem;
                transform: rotate(90deg);
            }
        }

        &-black,
        &-white {
            padding: 0.4rem 1rem;
            font-size: 1.3rem;
            line-height: 1.5;
            height: 2.8rem;
            border-radius: 0.8rem;
        }

        &-open {
            margin: 0 0.8rem 0 auto;
            padding: 0.2rem 0.4rem;
            font-size: 1.2rem;
            border-radius: 0.2rem;
            line-height: 1;
            height: fit-content;
        }
    }

    &-tit {
        margin: 0 0.2rem 0.4rem;
        height: 2.4rem;
        display: flex;
        align-items: center;
        font-weight: 400;
        font-size: 1.4rem;

        > .tooltip {
            margin-left: 0.4rem;
        }

        .btn-right {
            margin-left: auto;
        }
    }
    .btn-menu-expand + .sec-line {
        padding-top: 0;
    }

    .sec {
        &-line {
            padding: 2rem 2.2rem;
            border-bottom: 1px solid var(--border-color4);
        }

        &-form {
            .row {
                margin-top: 1.2rem;
                display: flex;
                align-items: center;
                min-height: 2rem;
                .tit {
                    font-size: 1.3rem;
                    margin-right: 0.6rem;
                }
                .txt {
                    color: var(--font-color3);
                    font-size: 1.1rem;
                    display: inline-block;

                    &-b {
                        font-size: 1.3rem;
                        margin-top: 0.4rem;
                    }
                    & + select,
                    &-b + select {
                        margin: 0 0.4rem;
                    }
                }

                &-wide {
                    flex-wrap: wrap;
                }
            }
            input[type="checkbox"].check-s + label {
                margin: 0.2rem 0 0 0.4rem;
                width: calc(100% - 2rem);
                vertical-align: text-top;
            }

            textarea {
                margin-top: 1rem;
                border-radius: 0;
            }
        }

        &-text {
            .text-wrap {
                font-size: 1.3rem;
                line-height: 1.53;
                color: var(--font-color3);
            }
        }
    }

    .clipboard-group {
        margin: 1rem 0;
        .btn-wrap {
            display: flex;
            > .btn-right {
                margin-left: auto;
            }
        }
    }

    .tab-group {
        width: calc(100% + 6rem - 4rem);
        margin-left: -1.2rem;

        &-btn {
            display: flex;
            
            > button {
                flex: 1;
                border: 0;
                padding: .8rem 0;
                font-size: 1.3rem;
                border-radius: 0;
                color: var(--font-color3);
                transition: color cubic-bezier(0.075, 0.82, 0.165, 1) .3s;
                border: 1px solid var(--border-color2);
                border-radius: 0.4rem;

                border-bottom: 0;
                
                &.active{
                    border: 0;
                    border-radius: 0;
                    border-bottom: 1px solid var(--font-color);
                    color: var(--font-color);
                    padding-bottom: 0.6rem;
                }
                
                &:hover {
                    background-color: transparent;
                    color: var(--font-color);
                }
            }
        }

        &-content {
            .link-text {
                padding: 1rem 1.4rem;
                display: block;
                line-height: 1.38;
                font-size: 1.3rem;

                &:hover {
                    color: var(--font-color-link);
                    text-decoration: underline;
                }
            }

            .qrcode-group {
                border: 1px dashed var(--border-color4);
                background-color: var(--btn-gray);
                padding: .8rem 1.4rem;
                font-size: 1.2rem;
                color: var(--font-color3);
                line-height: 1.33;
                
                .code-imgbox {
                    background-color: var(--bg-color);
                    border: 1px solid var(--border-color4);
                    width: 7.2rem;
                    height: 7.2rem;
                    margin-bottom: 0.8rem;
                    overflow: hidden;

                    > img {
                        width: 100%;
                    }
                }

                .desc {
                    margin-top: 0.4rem;

                }
            }
        }
    }
}
</style>

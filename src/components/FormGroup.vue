<template lang="">
    <div class="form-group-component">
        <div class="title-write-wrap">
            <p class="form-top-info">필수 입력사항</p>
            <div class="row">
                <h4 class="title required">설문명</h4>
                <div class="write-cont">
                    <label for="txt_bx" class="hide">설문명</label>
                    <input
                        type="text"
                        name="txt_bx"
                        id="txt_bx"
                        placeholder="설문명을 입력해주세요"
                        class="input-full"
                    />
                    <p class="form-info error">설문명을 입력하세요</p>
                </div>
            </div>
            <div class="row">
                <h4 class="title required">조사 기간</h4>
                <div class="write-cont">
                    <label for="txt_bx" class="hide">시작일시</label>
                    <input
                        type="date"
                        name="txt_bx"
                        id="txt_bx"
                        placeholder="시작일시"
                    />
                    <button type="button" class="btn btn-white btn-s btn-icon">
                        <i class="fa-regular fa-calendar-days icon"></i>
                        날짜 선택
                    </button>
                    <select name="selc" id="selc">
                        <option value="">00시</option>
                        <option value="1">1번</option>
                        <option value="2">2번</option>
                        <option value="3">3번</option>
                    </select>
                    <select name="selc" id="selc">
                        <option value="">00분</option>
                        <option value="1">1번</option>
                        <option value="2">2번</option>
                        <option value="3">3번</option>
                    </select>
                    <span class="tilde-txt">~</span>
                    <label for="txt_bx" class="hide">종료일시</label>
                    <input
                        type="date"
                        name="txt_bx"
                        id="txt_bx"
                        placeholder="종료일시"
                    />
                    <button type="button" class="btn btn-white btn-s btn-icon">
                        <i class="fa-regular fa-calendar-days icon"></i>
                        날짜 선택
                    </button>
                    <select name="selc" id="selc">
                        <option value="">00시</option>
                        <option value="1">1번</option>
                        <option value="2">2번</option>
                        <option value="3">3번</option>
                    </select>
                    <select name="selc" id="selc">
                        <option value="">00분</option>
                        <option value="1">1번</option>
                        <option value="2">2번</option>
                        <option value="3">3번</option>
                    </select>
                </div>
            </div>
        </div>
    </div>
    <div class="form-group-component">
        <div class="title-write-wrap">
            <div class="row">
                <h4 class="title">설문 종류</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex" id="rdc" checked />
                    <label for="rdc">일반설문</label>
                    <input type="radio" name="radio_ex" id="rd" />
                    <label for="rd">다면평가설문</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">설문 대상자</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex2" id="rdc2" checked />
                    <label for="rdc2">패널</label>
                    <input type="radio" name="radio_ex2" id="rd2" />
                    <label for="rd2">리스트</label>
                    <input type="radio" name="radio_ex2" id="rd3" />
                    <label for="rd3">dataSpring</label>
                    <input type="radio" name="radio_ex2" id="rd4" />
                    <label for="rd4">CHA University</label>
                    <p class="form-info">
                        와이즈인컴퍼니 보유 온라인패널을 이용한 조사
                        <a href="#" class="link">[자세히 보기]</a>
                    </p>
                </div>
            </div>
            <div class="row">
                <h4 class="title">전체 응답수</h4>
                <div class="write-cont">
                    <input
                        type="text"
                        name="txt_bx"
                        id="txt_bx"
                        class="input-s"
                    />
                    <span class="row-txt">명</span>
                </div>
            </div>
        </div>
    </div>
    <div class="form-group-component">
        <div class="title-write-wrap">
            <div class="row">
                <h4 class="title">링크주소</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex3" id="rdc3" checked />
                    <label for="rdc3">자동생성</label>
                    <input type="radio" name="radio_ex3" id="rd3" />
                    <label for="rd3">직접입력</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">
                    응답자 조회키
                    <i class="fa-solid fa-circle-info tooltip">
                        <span class="tooltip-desc">설문응답에 관련된 로그인 필요한</span>
                    </i>
                </h4>
                <div class="write-cont">
                    <input
                        type="text"
                        name="txt_bx"
                        id="txt_bx"
                        placeholder="30자까지 입력 가능합니다"
                    />
                </div>
            </div>
            <div class="row">
                <h4 class="title">접속 허용기기</h4>
                <div class="write-cont">
                    <input type="checkbox" name="ch" id="ch" checked />
                    <label for="ch">PC</label>

                    <input type="checkbox" name="ch" id="nch" />
                    <label for="nch">모바일</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">중복 응답제한</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex4" id="rdc4" />
                    <label for="rdc4">0단계 : 제한없음</label>
                    <input type="radio" name="radio_ex4" id="rd4" checked />
                    <label for="rd4">1단계 : 쿠키제한</label>
                    <input type="radio" name="radio_ex4" id="rd_4" />
                    <label for="rd_4">2단계 : 쿠키+IP제한</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">경고창 언어설정</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex5" id="rdc5" checked />
                    <label for="rdc5">한글</label>
                    <input type="radio" name="radio_ex5" id="rd5" />
                    <label for="rd5">영어</label>
                    <input type="checkbox" name="radio_ex5" id="ch" />
                    <label for="ch">2단계 : 쿠키+IP제한</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">자동문항 번호</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex6" id="rdc6" checked />
                    <label for="rdc6">설정 안함</label>
                    <input type="radio" name="radio_ex6" id="rd6" />
                    <label for="rd6">설정함</label>
                </div>
            </div>
            <div class="row">
                <h4 class="title">응답 수정</h4>
                <div class="write-cont">
                    <input type="radio" name="radio_ex7" id="rdc7" checked />
                    <label for="rdc7">꺼짐</label>
                    <input type="radio" name="radio_ex7" id="rd7" />
                    <label for="rd7">켜짐</label>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup></script>
<style lang="scss" scoped>
.form-group-component {
    border: 1px solid var(--border-color2);
    border-radius: 0.8rem;
    background-color: var(--bg-color);
    box-shadow: var(--shadow-1);
    padding: 3rem 9rem;
    margin-top: 1.3rem;

    &:first-child {
        margin-top: 3rem;
    }
}
</style>

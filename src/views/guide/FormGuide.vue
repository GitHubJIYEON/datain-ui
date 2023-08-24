<template>
    <div class="col">
        <div class="tit">1. 체크박스</div>
        <div class="cont">
            <input type="checkbox" name="ch" id="ch" checked />
            <label for="ch">체크</label>

            <input type="checkbox" name="nch" id="nch" />
            <label for="nch">체크x</label>
        </div>
    </div>
    <div class="col">
        <div class="tit">2. 체크박스(라벨x)</div>
        <div class="cont">
            <label for="ch">
                <input type="checkbox" name="ch" id="ch" checked />
            </label>

            <label for="nch">
                <input type="checkbox" name="nch" id="nch" />
            </label>
        </div>
    </div>
    <div class="col">
        <div class="tit">3. 라디오버튼</div>
        <div class="cont">
            <input type="radio" name="radio_ex" id="rdc" checked />
            <label for="rdc">체크</label>
            <input type="radio" name="radio_ex" id="rd" />
            <label for="rd">체크x</label>
        </div>
    </div>
    <div class="col">
        <div class="tit">4. 라디오버튼(라벨x)</div>
        <div class="cont">
            <label for="rdc">
                <input type="radio" name="radio_ex2" id="rdc2" checked />
            </label>
            <label for="rd">
                <input type="radio" name="radio_ex2" id="rd2" />
            </label>
        </div>
    </div>
    <div class="col">
        <div class="tit">5. 셀렉트박스</div>
        <div class="cont">
            <select name="selc" id="selc">
                <option value="">--- 선택 ---</option>
                <option value="1">1번</option>
                <option value="2">2번</option>
                <option value="3">3번</option>
            </select>
        </div>
    </div>
    <div class="col">
        <div class="tit">6. 텍스트박스</div>
        <div class="cont">
            <label for="txt_bx" class="hide">설문명</label>
            <input
                type="text"
                name="txt_bx"
                id="txt_bx"
                placeholder="설문명을 입력해주세요"
            />
            <hr />
            <label for="txt_bx">설문명</label>
            <input
                type="text"
                name="txt_bx"
                id="txt_bx"
                placeholder="설문명을 입력해주세요"
            />
        </div>
    </div>
    <div class="col">
        <div class="tit">7. 텍스트박스 (필수입력값), 경고문구</div>
        <div class="cont">
            <label for="txt_bx" class="required">설문명</label>
            <div class="wrap">
                <!-- <input type="text" name="txt_bx" id="txt_bx" value="설문명을 입력해주세요"/> -->
                <p class="form-info error">설문명을 입력하세요</p>
            </div>
        </div>
    </div>
    <div class="col">
        <div class="tit">8. 버튼</div>
        <div class="cont">
            <button type="button" class="btn">버튼</button>
            <button type="button" class="btn btn-black">확인</button>
            <button type="button" class="btn btn-white">취소</button>
            <button type="button" class="btn btn-gray">-</button>
            <hr />
            <a href="#" class="btn">버튼</a>
            <a href="#" class="btn btn-black">확인</a>
            <a href="#" class="btn btn-white">취소</a>
            <a href="#" class="btn btn-gray">-</a>
            <hr />
            <button class="btn-icon type2">
                <i class="fa-solid fa-magnifying-glass icon"></i>
                검색
            </button>
            <button class="btn-icon btn-s">
                <i class="fa-solid fa-magnifying-glass icon"></i>
                검색
            </button>
        </div>
    </div>
    <div class="col">
        <div class="tit">9. 버튼 스타일링</div>
        <div class="cont">
            <button type="button" class="btn btn-round">버튼</button>
            <button type="button" class="btn btn-round btn-full btn-white">
                버튼
            </button>
            <button type="button" class="btn btn-full btn-align-l">
                <b>+ </b>시작하기
            </button>
            <button type="button" class="btn btn-gray btn-full btn-align-l">
                <i class="icon">👋🏻 </i>신규 설문 등록
            </button>
        </div>
    </div>
    <div class="col">
        <div class="tit">10. 이전 / 다음 버튼</div>
        <div class="cont">
            <button type="button" class="btn-move prev">이전</button>
            <button type="button" class="btn-move next">다음</button>
            <button type="button" class="btn-move prev text">이전</button>
            <button type="button" class="btn-move next text">다음</button>
        </div>
    </div>
    <div class="col">
        <div class="tit">11. 텍스트 에어리어</div>
        <div class="cont">
            <textarea name="" id="" placeholder="내용을 입력하세요"></textarea>
        </div>
    </div>
    <div class="col">
        <div class="tit">12. 툴팁</div>
        <div class="cont">
            <i class="fa-solid fa-circle-info tooltip">
                <span class="tooltip-desc">설문응답에 관련된 로그인 필요한</span>
            </i>
        </div>
    </div>
    <!-- <div class="col">
        <div class="tit">추후 추가 예정...</div>
        <div class="cont"></div>
    </div> -->
    <div class="col col-4">
        <div class="tit">[활용예시 1] 새로운 설문 작성하기 페이지</div>
        <div class="cont">
            <div class="title-write-wrap">
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
                    <h4 class="title">보기문항</h4>
                    <div class="write-cont">
                        <label for="txt_bx" class="hide">보기문항</label>
                        <input
                            type="text"
                            name="txt_bx"
                            id="txt_bx"
                            placeholder="보기문항을 입력해주세요"
                        />
                        <button type="button" class="btn btn-white btn-s">
                            이미지 업로드
                        </button>
                        <button type="button" class="btn btn-white btn-s">
                            <i class="fa-solid fa-image icon"></i> 이미지 업로드
                        </button>
                        <button
                            type="button"
                            class="btn btn-white btn-s btn-icon"
                        >
                            <i class="fa-solid fa-image icon"></i> 이미지 업로드
                        </button>
                        <button
                            type="button"
                            class="btn btn-white btn-s btn-icon"
                        >
                            <i class="fa-regular fa-calendar-days icon"></i>
                            이미지 업로드
                        </button>
                        <select name="selc" id="selc">
                            <option value="">--- 선택 ---</option>
                            <option value="1">1번</option>
                            <option value="2">2번</option>
                            <option value="3">3번</option>
                        </select>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup></script>

<style lang="scss" scoped>
// 이 페이지 내에서만 사용할 스타일.
label + input {
    margin-left: 1rem;
}

label + label {
    margin-left: 1rem;
}

button + button,
a.btn + a.btn {
    margin-left: 1rem;
}
button.btn-full {
    margin: 0;
    margin-top: 1rem;
}

.title-write-wrap {
    margin-top: 2rem;
}

.tooltip {
    margin: auto;
}
</style>

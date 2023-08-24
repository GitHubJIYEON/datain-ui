<template>
    <footer id="footer">
        <div class="banner">
            <div class="l-wrap">
                <p class="banner-top-title">데이터인에서 만나는 세상 모든 편리한,  전문 기능 포함</p>
                <h3 class="banner-title">데이터인</h3>
            </div>
            <div class="r-wrap">
                <img src="@/assets/img/sub/footer-banner-img.png" alt="데이터인">
            </div>
        </div>
    </footer>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
    footer {
        height: 18rem;
        background-color: var(--primary-color);
        display: flex;
        align-items: center;
        justify-content: center;

        > .banner {
            user-select: none;
            width: 61.8rem;
            display: flex;
            justify-content: space-between;
            color: var(--font-color2);

            > .l-wrap {
                margin-top: 1.8rem;
                font-weight: 200;
                letter-spacing: -0.05rem;
            }
            > .r-wrap {

            }

            .banner-top-title{
                line-height: 167%;
                font-size: 1.8rem;
                margin-bottom: 0.4rem;
            }
            .banner-title{
                font-size: 3.2rem;
                line-height: 1;
                font-weight: 300;
            }
        }
    }
</style>
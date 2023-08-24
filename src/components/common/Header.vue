<template>
    <header id="header">
        <h1 class="logo">
            <a href="/">
                <img
                    src="@/assets/img/common/logo-purple.svg"
                    class="logo-img"
                    alt="데이터인"
                />
            </a>
        </h1>
        <div class="toggle-nav-group">
            <button class="toggle-btn nav">
                네비게이션토글
                <!-- <img
                    src="@/assets/img/common/angle-up-down.svg"
                    alt="네비게이션 토글 버튼"
                /> -->
            </button>
            <nav class="nav-group">
                <a href="#" class="nav-link">설문</a>
                <a href="#" class="nav-link">모니터링</a>
                <a href="#" class="nav-link">분석</a>
                <a href="#" class="nav-link">통합리포팅</a>
                <a href="#" class="nav-link">텍스트인</a>
            </nav>
        </div>
        <h2 class="page-main-title">설문</h2>
        <nav class="r-tab-group">
            <ul>
                <li>
                    <a href="#" class="tab active"
                        ><i class="fa-solid fa-list"></i>설문</a
                    >
                </li>
                <li>
                    <a href="#" class="tab"
                        ><i class="fa-solid fa-route"></i>로직</a
                    >
                </li>
                <li>
                    <a href="#" class="tab disabled"
                        ><i class="fa-solid fa-desktop"></i>테스트</a
                    >
                </li>
                <li>
                    <a href="#" class="tab"
                        ><i class="fa-solid fa-database"></i>데이터</a
                    >
                </li>
            </ul>
        </nav>
        <div class="toggle-nav-group right">
            <button class="toggle-btn more">더보기</button>
        </div>
    </header>
</template>

<script setup></script>

<style lang="scss" scoped>
#header {
    background-color: var(--bg-color);
    display: flex;
    position: fixed;
    width: 100%;
    align-items: center;
    border-bottom: 1px solid var(--border-color);
    padding: 0 28px;
    height: 66px;
    z-index: 999;

    .logo {
        font-size: 0;

        .logo-img {
            width: 131px;
            height: auto;
        }
    }

    .page-main-title {
        font-size: 2.4rem;
        color: var(--primary-color);
        margin-left: 16rem;

        &::before {
            content: "[";
        }

        &::after {
            content: "]";
        }
    }

    .toggle-nav-group {
        position: relative;

        &.right {
            margin-left: auto;
        }

        > .toggle-btn {
            font-size: 0;
            width: 3rem;
            height: 3rem;

            &.nav {
                border-radius: 50%;
                margin-left: 2rem;
                background: url("@/assets/img/common/angle-up-down.svg")
                    no-repeat center center;

                &:hover {
                    background-color: #eee;
                }
            }
            &.more {
                background: url("@/assets/img/common/ellipsis-vertical.svg")
                    no-repeat center center;
                border: 0;
            }
        }
        > .nav-group {
            &.active {
                display: block;
            }

            display: none;
            width: 21.5rem;
            position: absolute;
            background-color: var(--bg-color);
            border: 1px solid var(--border-color2);
            padding: 2.4rem;
            border-radius: 1.5rem;
            box-shadow: 0px 6px 12px 0px rgba(0, 0, 0, 0.06);

            > .nav-link {
                display: block;
                font-size: 1.8rem;
                font-weight: 500;
                line-height: 133%;
                margin-top: 1.4rem;
                letter-spacing: -0.05rem;
                background: url("@/assets/img/common/arrow-right.svg") no-repeat
                    center right;

                &:first-child {
                    margin-top: 0;
                }
            }
        }
    }

    .r-tab-group {
        position: absolute;
        right: 38rem;
        bottom: 0;

        > ul {
            list-style: none;
            display: flex;
        }

        .tab {
            border: 1px solid var(--border-color2);
            border-radius: 0.8rem 0.8rem 0 0;
            border-bottom: none;
            padding: 1.2rem 1.8rem .8rem;
            color: var(--font-color3);
            display: block;
            transition: all 0.3s ease-out;
            line-height: 1.33;
            margin-left: 0.4rem;

            > i {
                font-size: 1.3rem;
                vertical-align: middle;
                display: inline-block;
                margin-top: -0.2rem;
                margin-right: 0.8rem;
            }

            &.active,
            &:hover {
                border: 1px solid var(--primary-color);
                color: var(--primary-color);
                border-bottom: 0;
            }

            &.disabled {
                background-color: var(--border-color);
                color: var(--icon-color);

                &:hover {
                    border-color: var(--border-color2);
                }
            }
        }
    }
}
</style>

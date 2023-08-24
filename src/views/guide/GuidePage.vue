<template>
    <div class="guide-page container">
        <div class="content-list">
            <a href="#content1">Col Guide</a> / 
            <a href="#content2">Form Style Guide</a> / 
            <a href="#content3">Component Style Guide</a>
        </div>
        <h3 class="page-title" id="content1">Col Guide</h3>
        <div class="page-content">
            <ColGuide />
        </div>

        <h3 class="page-title" id="content2">Form Style Guide</h3>
        <form action="">
            <div class="page-content">
                <FormGuide />
            </div>
        </form>

        <h3 class="page-title" id="content3">Component Style Guide</h3>
        <form action="">
            <div class="page-content">
                <ComponentGuide />
            </div>
        </form>

        <a href="#" class="up-btn"><i class="fa-solid fa-angle-up"></i><br>TOP</a>
    </div>
</template>

<script setup>
import ColGuide from "./ColGuide.vue";
import ComponentGuide from "./ComponentGuide.vue";
import FormGuide from "./FormGuide.vue";
</script>

<style lang="scss">
.guide-page {
    margin-top: -10rem;

    .up-btn {
        position: fixed;
        right: 3rem;
        bottom: 3rem;
        display: block;
        padding-top: .6rem;
        line-height: 1;
        width: 5rem;
        height: 5rem;
        background-color: var(--bg-color);
        color: var(--primary-color);
        border-radius: 50%;
        text-align: center;
        box-shadow: 3px 3px 5px #33333330;
        border: 1px solid var(--border-color);
        font-weight: 600;

    }
    
    .content-list {
        margin-top: 10rem;
        > a {
            color: var(--primary-color);
            text-decoration: underline;
        }
    }

    .page-title {
        font-size: 3.4rem;
        margin-top: 10rem;
        text-align: left;
    }

    .page-content {
        display: flex;
        flex-wrap: wrap;
        gap: 1rem;
        width: calc(100% + 1rem);

        > .col {
            width: calc(25% - 1rem);
            margin-top: 1.5rem;
            border: 1px solid #ddd;
            border-radius: 0.5rem;
            padding: 1.8rem;

            &-4 {
                width: calc(100% - 1rem);
            }

            &-3 {
                width: calc(100% / 3 - 1rem);
            }

            &-2 {
                width: calc(50% - 1rem);
            }

            > .tit {
                font-size: 1.8rem;
                margin-bottom: 1rem;
                font-weight: 500;
                color: #666;
                letter-spacing: -0.06rem;
                border-bottom: 1px solid #ddd;
                padding-bottom: 0.4rem;
                margin-bottom: 1.2rem;
            }
            > .cont {
                padding-left: 1rem;
                min-height: 5rem;
            }
        }
    }
}
</style>

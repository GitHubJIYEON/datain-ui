<template>
    <LeftMenu />
    <div class="container container-type2">
        <TopTitle />
        container
    </div>
    <RightMenu/>
</template>
<script setup>
import LeftMenu from "@/components/common/LeftMenu.vue";
import TopTitle from "@/components/common/TopTitle.vue";
import RightMenu from "@/components/common/RightMenu.vue";
</script>
<style lang="scss" scoped>
.container{
    padding-top: 7.3rem;
}
</style>

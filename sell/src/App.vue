<template>
    <div id="heheda">
        <v-header></v-header>
        <div class="tab">
            <div class="tab-item">
                <a v-link="{path:'/goods'}">商品</a></div>
            <a v-link="{path:'/ratings'}">评论</a></div>
        <a v-link="{path:'/seller'}">商家</a></div>
    <router-view></router-view>
    </div>
    <div class="content"> I am content</div>
    </div>
</template>
<script>
    import header from './components/header/header.vue';
    export default{
        components: {
            'v-header': header
        }
    };
</script>
<style lang="stylus" rel="stylesheet/stylus">
    #heheda
        .tab
            display: flex
            width: 100%
            height: 40px
        .tab-item
            flex: 1
            text-align: center


</style>

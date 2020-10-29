<style lang="less">
    .g-input{
        border: 1px solid rgb(150, 150, 150);
        border-radius: 10px;
        outline: none;
        padding-left: 5px;
        height: 25px;
        width: 200px;
        margin: 6px;
    }
</style>

<template>
    <div>
        <input
            ref="gInput"
            @focus="gFocusInput"
            :value="value"
            :placeholder="placeholder"
            class="g-input" 
            type="text"
        >
    </div>
</template>

<script>
export default {
    data(){
        return {}
    },
    props: ["value", "placeholder", "width", "backgroundColor"],
    components:{

    },
    mounted(){

    },
    methods: {
        gFocusInput(){
            this.$refs.gInput.style.border = '1px solid rgb(3,169,244)'
        }
    }
}
</script>
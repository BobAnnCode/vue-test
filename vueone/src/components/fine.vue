<template>
    <div class="fine">
        <button name="button" type="button" @click="fine">fine</button>
    </div>
</template>

<script>
    export default {
        methods:{
            fine:function () {
                window.alert("fine")
            }
        }
    }
</script>

<style scoped>

</style>

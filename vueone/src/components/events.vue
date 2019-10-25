<template lang="html">
    <div class="events">
        <button name="button" type="button" @click="msg">test</button>
    </div>
</template>

<script>
    export default {
        methods:{
            msg:function () {
                window.console.log(Math.random());
                window.alert("fine");
            }
        }
    }
</script>

<style lang="css">

</style>

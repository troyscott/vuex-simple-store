// ShowGreetingsComponent.vue
<template>
<div>
<h1>{{ msg }}</h1>
<div>The message was changes {{ counter }} times </div>
</div>
</template>
<script>
import { mapGetters } from 'vuex'
export default {
    computed: mapGetters({
        msg: 'getMessage',
        counter: 'getCounter'
    })
}
</script>
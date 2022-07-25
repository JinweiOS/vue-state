<template>
    <div>{{sharedStore.message}}</div>
</template>
<script>
import store from '../easy-store'
export default {
    name: 'ViewOne',
    data: function() {
        return {
            sharedStore: store.state
        }
    },
    mounted() {
        setTimeout(() => store.setMessageAction('哈哈哈哈'), 3000)
    }
}
</script>
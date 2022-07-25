<template>
    <div>{{sharedStore.message}}</div>
</template>
<script>
import store from '../easy-store'
export default {
    name: 'ViewTwo',
    data: function() {
        return {
            sharedStore: store.state
        }
    }
}
</script>
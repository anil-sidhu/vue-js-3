<template>
<div>
<h3 >Bruce</h3>
<h3>Peter</h3>
<h3 v-bind="$attrs">Tony</h3>
</div>
</template>
<script>
export default {
    name:'User',
    inheritAttrs:false
}
</script>
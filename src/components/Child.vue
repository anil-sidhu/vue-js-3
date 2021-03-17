<template>
<div class="cart">
    <header>
        <slot name="header">Default Data</slot>
    </header>
    <content>
        <slot name="main">Default Data</slot>
    </content>
    <footer>
        <slot name="footer">Default Data</slot>
    </footer>

</div>
</template>

<script>
export default {
    name: 'Child',
}
</script>
<style>
.cart{
    border: 1px solid;
    width: 131px;
    padding: 20px;
    margin: 20px;
    text-align: center;
}
</style>

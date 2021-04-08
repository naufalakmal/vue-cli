<template>
    <h1>Hello, {{ name }}</h1>
</template>

<script>
export default {
    // harus sesuai dengan index.js
    props: ['name']
}
</script>
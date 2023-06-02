<template>
    <div>
        {{ filme.year }} : {{ filme.name }} ({{ filme.awards }})
    </div>
</template>

<script>
export default {
    props: {
        filme: {}
    },
    data() {
        return {

        }
    }
}
</script>
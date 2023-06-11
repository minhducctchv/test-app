<template>
    <div>
        Xin chao {{ computedName }}
    </div>
</template>

<script setup>
import { ref, computed, unref } from 'vue'

const bien1 = ref('giatri1')
const bien2 = ref('giatri2')
const bien3 = ref('giatri3')

const computedName = computed(() => {
    return unref(bien1) + unref(bien2) + unref(bien3)
})
</script>

<style lang="scss" scoped></style>
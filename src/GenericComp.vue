<script lang="ts" generic="Data" setup>
    import { computed } from 'vue';
    import type { Ref } from 'vue';

    const props = defineProps<{
        valueFactory: () => Data;
    }>();

    const result: Ref<Data> = computed(() => {
        return props.valueFactory();
    });

</script>

<template>
    <div>
        <slot :result="result" />
    </div>
</template>

<template>
    <rd-checkbox-group
        v-bind="$attrs"
    >
        <rd-checkbox
            v-for="(item, index) in enumOptions"
            :key="index"
            :label="item.value"
        >
            {{ item.label }}
        </rd-checkbox>
    </rd-checkbox-group>
</template>

<script>
export default {
    name: 'CheckboxesWidget',
    props: {
        enumOptions: {
            default: () => [],
            type: [Array]
        }
    }
};
</script>

<template>
    <v-text-field clearable :label="label" color="purple" variant="underlined" class="mb-3"></v-text-field>
</template>
<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    props: {
        label: {
            required: true,
            type: String
        }
    }
});

</script>
<template>
    <v-btn :prepend-icon="prependIcon" :size="size" :color="color">
        {{ label }}
    </v-btn>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    props: {
        label: {
            required: true,
            type: String
        },
        prependIcon: {
            type: String
        },
        size: {
            type: String
        },
        color: {
            type: String
        }
    }
});
</script>
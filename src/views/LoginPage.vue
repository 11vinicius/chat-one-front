<template>
    <v-container>
        <v-card class="mx-auto pa-10 mt-16" max-width="650">
            <v-form>
                <v-img src="@/assets/logo.png" class="mb-10 logoLogin"></v-img>
                <TextField label="Email" />
                <TextField label="password" />
                <ButtonComponent label="Entrar" color="purple" size="large" />
            </v-form>
        </v-card>
    </v-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import { useAuth } from '@/store';

import TextField from '@/components/TextFieldComponent.vue';
import ButtonComponent from '@/components/ButtonComponent.vue';

export default defineComponent({
    components: {
        TextField,
        ButtonComponent
    },

    setup() {
        const authStore = useAuth();

        return {
            authStore
        }
    }
})
</script>

<style scoped>
.logoLogin {
    max-height: 350px;
}
</style>
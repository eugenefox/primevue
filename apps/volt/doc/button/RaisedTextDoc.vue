<template>
    <DocSectionText v-bind="$attrs">
        <p>Text buttons can be displayed elevated with the <i>raised</i> option.</p>
    </DocSectionText>
    <div class="card flex justify-center flex-wrap gap-4">
        <Button label="Primary" variant="text" raised />
        <SecondaryButton label="Secondary" variant="text" raised />
        <ContrastButton label="Contrast" variant="text" raised />
        <DangerButton label="Danger" variant="text" raised />
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import Button from '@/volt/Button.vue';
import ContrastButton from '@/volt/ContrastButton.vue';
import DangerButton from '@/volt/DangerButton.vue';
import SecondaryButton from '@/volt/SecondaryButton.vue';
import { ref } from 'vue';

const code = ref(`
<template>
   <div class="card flex justify-center flex-wrap gap-4">
        <Button label="Primary" variant="text" raised />
        <SecondaryButton label="Secondary" variant="text" raised />
        <ContrastButton label="Contrast" variant="text" raised />
        <DangerButton label="Danger" variant="text" raised />
    </div>
</template>

<script setup lang="ts">
import Button from '@/volt/Button.vue';
import ContrastButton from '@/volt/ContrastButton.vue';
import DangerButton from '@/volt/DangerButton.vue';
import SecondaryButton from '@/volt/SecondaryButton.vue';
<\/script>
`);
</script>

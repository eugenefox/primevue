<template>
    <DocSectionText v-bind="$attrs">
        <p>
            The position of the labels relative to the meters is defined using the <i>labelPosition</i> property. The default orientation of the labels is horizontal, and the vertical alternative is available through the
            <i>labelOrientation</i> option.
        </p>
    </DocSectionText>
    <div class="card">
        <MeterGroup :value="value" labelPosition="start" labelOrientation="vertical" />
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import MeterGroup from '@/volt/MeterGroup.vue';
import { ref } from 'vue';

const value = ref([
    { label: 'Apps', color: '#34d399', value: 16 },
    { label: 'Messages', color: '#fbbf24', value: 8 },
    { label: 'Media', color: '#60a5fa', value: 24 },
    { label: 'System', color: '#c084fc', value: 10 }
]);

const code = ref(`
<template>
    <div class="card">
        <MeterGroup :value="value" labelPosition="start" labelOrientation="vertical" />
    </div>
</template>

<script setup lang="ts">
import MeterGroup from '@/volt/MeterGroup.vue';
import { ref } from 'vue';

const value = ref([
    { label: 'Apps', color: '#34d399', value: 16 },
    { label: 'Messages', color: '#fbbf24', value: 8 },
    { label: 'Media', color: '#60a5fa', value: 24 },
    { label: 'System', color: '#c084fc', value: 10 }
]);
<\/script>
`);
</script>

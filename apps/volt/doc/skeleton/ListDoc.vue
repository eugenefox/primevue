<template>
    <DocSectionText v-bind="$attrs">
        <p>Sample List implementation using different Skeleton components and Tailwind CSS utilities.</p>
    </DocSectionText>
    <div class="card">
        <div class="rounded-sm border border-surface-200 dark:border-surface-700 p-6 bg-surface-0 dark:bg-surface-900">
            <ul class="m-0 p-0 list-none">
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import Skeleton from '@/volt/Skeleton.vue';
import { ref } from 'vue';

const code = ref(`
<template>
    <div class="card">
        <div class="rounded-sm border border-surface-200 dark:border-surface-700 p-6 bg-surface-0 dark:bg-surface-900">
            <ul class="m-0 p-0 list-none">
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li class="mb-4">
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="flex">
                        <Skeleton shape="circle" size="4rem" class="mr-2"></Skeleton>
                        <div class="self-center" style="flex: 1">
                            <Skeleton width="100%" class="mb-2"></Skeleton>
                            <Skeleton width="75%"></Skeleton>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script setup lang="ts">
import Skeleton from '@/volt/Skeleton.vue';
<\/script>
`);
</script>

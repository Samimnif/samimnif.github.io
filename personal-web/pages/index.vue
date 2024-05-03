<script lang="ts" setup>
import { Icon } from '@iconify/vue';
</script>
<template>

    <UContainer>
        <Placeholder class="h-32" />
        <br>
        <UCard>
            <template #header>
                <Placeholder class="h-8" />
                <UAvatar size="3xl" src="https://avatars.githubusercontent.com/u/66852892?v=4" alt="Avatar" />
                <h1>Hi! My name is <UBadge size="lg">Sami Mnif</UBadge>
                </h1>
            </template>

            <Placeholder class="h-32" />
            <h3>I am 4th year Systems Software Engineering Student at Carleton University</h3>
            <template #footer>
                <Placeholder class="h-8" />
                <div class="flex justify-center">
                    <ULink to="https://github.com/Samimnif/" active-class="text-primary"
                        inactive-class="text-gray-500 dark:text-gray-400 hover:text-gray-700 dark:hover:text-gray-200"
                        target="_blank">
                        <Icon icon="mdi:github" width="48" height="48" />
                    </ULink>
                    <ULink to="https://www.linkedin.com/in/sami-mnif-64346b178/" active-class="text-primary"
                        inactive-class="text-gray-500 dark:text-gray-400 hover:text-gray-700 dark:hover:text-gray-200"
                        target="_blank">
                        <Icon icon="mdi:linkedin" width="48" height="48" />
                    </ULink>
                </div>
            </template>
        </UCard>
    </UContainer>

</template>

<template>
    <UContainer>
        <Placeholder class="h-32" />
            <UCard v-for="exp in experiences" :key="exp.title" cols="3" sm="1">
                <template #header>
                    <Placeholder class="h-8" />
                    <h1>{{ exp.title }}</h1>
                </template>

                <Placeholder class="h-32" />
                <h4>{{ exp.description }}</h4>
            </UCard>
    </UContainer>
</template>

<script>
import experienceData from "/static/experience.json"

export default {
    data() {
        return { experiences: experienceData }
    }
}
</script>
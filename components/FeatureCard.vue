<template>
    <v-card :id="`feature-${feature.id}`" class="feature-card pa-6" flat>
        <div class="d-flex align-start">
            <v-avatar :color="feature.color" size="64" class="me-4">
                <v-icon :icon="feature.icon" color="white" size="32" />
            </v-avatar>

            <div class="flex-grow-1">
                <h3 class="text-h5 font-weight-bold mb-3">
                    {{ feature.title }}
                </h3>
                <p class="text-body-1 text-medium-emphasis">
                    {{ feature.description }}
                </p>
            </div>
        </div>
    </v-card>
</template>

<script setup lang="ts">
interface Feature {
    id: string
    title: string
    description: string
    icon: string
    color: string
}

defineProps<{
    feature: Feature
}>()
</script>

<style scoped>
.feature-card {
    height: 100%;
    transition: transform 0.2s ease;
}

.feature-card:hover {
    transform: translateY(-4px);
}
</style>
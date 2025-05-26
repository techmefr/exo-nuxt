<template>
    <ClientOnly>
        <v-container class="pa-0" fluid>
            <section class="text-center py-8">
                <v-img
src="https://via.placeholder.com/400x200/f5f5f5/999999?text=Hero+Image" width="400"
                    class="mx-auto mb-6" />

                <h1 class="text-h2 font-weight-bold mb-4">
                    Figma Design System
                </h1>
                <p class="text-h6 mb-6 text-medium-emphasis">
                    No matter what project you're working on, we've got you covered with the best wireframe kits for any
                    platform.
                </p>
                <v-btn color="primary" size="large" class="mb-8">
                    Download for Mac
                </v-btn>

                <v-row justify="center" class="align-center">
                    <v-col cols="auto">
                        <span class="text-caption">v1.0.0.2</span>
                    </v-col>
                    <v-divider vertical class="mx-4" />
                    <v-col cols="auto">
                        <span class="text-caption">macOS 15+</span>
                    </v-col>
                    <v-divider vertical class="mx-4" />
                    <v-col cols="auto">
                        <span class="text-caption">Works via Chrome</span>
                    </v-col>
                </v-row>
            </section>

            <div class="text-center my-8">
                <v-chip color="success" size="small">
                    Advertising
                </v-chip>
            </div>

            <section class="build-section text-center mb-12">
                <h2 class="text-h3 font-weight-bold mb-4">
                    Build your website with Blank
                </h2>
                <p class="text-h6 text-medium-emphasis mb-8">
                    No matter what project you're working on, we've got you covered with the best wireframe kits for any
                    platform.
                </p>

                <v-row justify="center">
                    <v-col v-for="feature in features" :key="feature.id" cols="12" md="6">
                        <FeatureCard :feature="feature" />
                    </v-col>
                </v-row>
            </section>

            <div class="text-center my-8">
                <v-chip color="success" size="small">
                    Advertising
                </v-chip>
            </div>

            <section class="final-section text-center">
                <h2 class="text-h3 font-weight-bold mb-4">
                    Build your website with Blank
                </h2>
                <p class="text-h6 text-medium-emphasis">
                    No matter what project you're working on, we've got you covered with the best wireframe kits for any
                    platform.
                </p>
            </section>
        </v-container>
    </ClientOnly>
</template>

<script setup lang="ts">
definePageMeta({
    ssr: false
})

interface Feature {
    id: string
    title: string
    description: string
    icon: string
    color: string
}

const features: Feature[] = [
    {
        id: 'design-system',
        title: 'Design system',
        description: 'Fully customizable and neatly organized components will help you work faster without limiting creative freedom.',
        icon: 'mdi-palette',
        color: 'pink'
    },
    {
        id: 'components',
        title: 'Components',
        description: 'Fully customizable and neatly organized components will help you work faster without limiting creative freedom.',
        icon: 'mdi-view-grid',
        color: 'purple'
    },
    {
        id: 'auto-layout',
        title: 'Auto layout',
        description: 'Fully customizable and neatly organized components will help you work faster without limiting creative freedom.',
        icon: 'mdi-auto-fix',
        color: 'green'
    },
    {
        id: 'lifetime-updates',
        title: 'Lifetime updates',
        description: 'Fully customizable and neatly organized components will help you work faster without limiting creative freedom.',
        icon: 'mdi-star',
        color: 'purple'
    }
]
</script>

<style scoped>
.build-section {
    max-width: 800px;
    margin: 0 auto;
}

.final-section {
    max-width: 600px;
    margin: 0 auto;
    padding-bottom: 4rem;
}
</style>
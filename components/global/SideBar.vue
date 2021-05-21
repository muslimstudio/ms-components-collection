<template>
  <div class="bg-gray-100 dark:bg-midnight">
    <template>
      <div class="pt-8 px-3 flex">
        <div class="hidden md:block flex-none h-full overflow-y-auto top-0 sticky max-h-screen">
          <nav class="w-56 pt-6 pb-12 px-3 h-full">
            <h1 class="text-gray-400 dark:text-gray-500">Button</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
            <h1 class="text-gray-400 dark:text-gray-500">Test</h1>
          </nav>
        </div>
        <div>
          <section class="mb-12 max-w-full">
            <h1 class="mb-2 text-3xl text-gray-800 dark:text-gray-500">Button</h1>
            <div class="bg-white dark:bg-gray-900 p-6 rounded border-gray-300 dark:border-gray-900 border">
              <slot />
            </div>
          </section>
          <!-- <CanvasSection
            v-for="section in configTransformed"
            :key="section.title"
            :title="section.title"
            :id="section.title"
          >
            <Intersect
              :threshold="[0.0]"
              rootMargin="-40% 0px -60% 0px"
              @enter="setActiveSection(section)"
              @leaave="setActiveSection(null)"
            >
              <component
                :is="sectionComponent(section.component)"
                :data="section.data"
                :config="config"
              />
            </Intersect>
          </CanvasSection> -->
        </div>
      </div>
    </template>
  </div>
</template>

<script>
export default {
  components: {
  },
  props: {
    darkMode: {
      type: Boolean,
      required: false
    }
  },
  data () {
    return {
      
    }
  },
}
</script>
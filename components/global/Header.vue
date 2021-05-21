<template>
  <header>
    <div class="flex justify-between items-center bg-white dark:bg-gray-800 border-b dark:border-gray-800 p-4 text-gray-700 dark:text-gray-500 font-bold">
      <span class="text-xl">MS Components Collections</span>
      <div>
        <ToggleSwitch/>
      </div>
    </div>
  
  </header>
</template>

<script>
import ToggleSwitch from "~/components/organisms/ToggleSwitch";
export default {
  props: {
    darkMode: {
      type: Boolean,
      required: false
    }
  },
  components: {
    ToggleSwitch
  }
}
</script>
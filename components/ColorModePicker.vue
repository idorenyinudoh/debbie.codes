<template>
  <div class="text-center">
    <div>
      <ul>
        <li v-for="color of colors" :key="color" class="inline-block p-2">
          <component
            :is="`icon-${color}`"
            :class="getClasses(color)"
            @click="$colorMode.preference = color"
          />
        </li>
      </ul>
      <p>
        <ColorScheme placeholder="..." tag="span">
          Color mode: <b>{{ $colorMode.preference }}</b>
          <span v-if="$colorMode.preference === 'system'">
            (<i>{{ $colorMode.value }}</i> mode detected)
          </span>
        </ColorScheme>
      </p>
    </div>
  </div>
</template>

<script>
  import IconSystem from '@/assets/icons/system.svg?inline'
  import IconLight from '@/assets/icons/light.svg?inline'
  import IconDark from '@/assets/icons/dark.svg?inline'
  import IconSepia from '@/assets/icons/sepia.svg?inline'

  export default {
    components: {
      IconSystem,
      IconLight,
      IconDark,
      IconSepia
    },
    data() {
      return {
        colors: ['system', 'light', 'dark', 'sepia']
      }
    },
    methods: {
      getClasses(color) {
        // Does not set classes on ssr preference is system (because we know them on client-side)
        if (this.$colorMode.unknown) {
          return {}
        }
        return {
          prefered: color === this.$colorMode.preference,
          selected: color === this.$colorMode.value
        }
      }
    }
  }
</script>

<style scoped>
  p {
    margin: 0;
    padding-top: 5px;
    padding-bottom: 20px;
  }
  .feather {
    position: relative;
    top: 0px;
    cursor: pointer;
    padding: 7px;
    background-color: var(--bg-secondary);
    border: 2px solid var(--border-color);
    margin: 0;
    border-radius: 5px;
    transition: all 0.1s ease;
    width: 40px;
    height: 40px;
    will-change: transform;
    transform: translateZ(0);
  }
  .feather:hover {
    top: -3px;
  }
  .feather.prefered {
    border-color: var(--color-primary);
    top: -3px;
  }
  .feather.selected {
    color: var(--color-primary);
  }
</style>

<template>
  <footer>
    <div class="max-w-7xl mx-auto py-12 px-4 overflow-hidden sm:px-6 lg:px-8">
      <nav
        class="-mx-5 -my-2 flex flex-wrap justify-center"
        aria-label="Footer"
      >
        <div class="px-5 py-2">
          <NuxtLink
            to="/about"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            About
          </NuxtLink>
        </div>
        <div class="px-5 py-2">
          <NuxtLink
            to="/blog"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Blog
          </NuxtLink>
        </div>

        <div class="px-5 py-2">
          <NuxtLink
            to="/resources/guest-live-streams"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Streams
          </NuxtLink>
        </div>

        <div class="px-5 py-2">
          <NuxtLink
            to="/resources/interviews"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Interviews
          </NuxtLink>
        </div>

        <div class="px-5 py-2">
          <NuxtLink
            to="/resources/podcasts"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Podcasts
          </NuxtLink>
        </div>

        <div class="px-5 py-2">
          <NuxtLink
            to="/resources"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Resources
          </NuxtLink>
        </div>

        <div class="px-5 py-2">
          <NuxtLink
            to="/contact"
            class="text-base text-gray-800 dark:text-gray-400 hover:text-primary"
          >
            Contact
          </NuxtLink>
        </div>
      </nav>
      <div class="mt-8 flex justify-center space-x-6">
        <a
          href="https://twitter.com/debs_obrien"
          aria-label="twitter"
          target="_blank"
          rel="nofollow noopener noreferrer"
        >
          <IconTwitter class="h-10 w-10 fill-current" />
        </a>

        <a
          href="https://www.linkedin.com/in/debbie-o-brien-1a199975/"
          target="_blank"
          rel="nofollow noopener noreferrer"
          aria-label="linkedIn"
        >
          <IconLinkedIn class="h-10 w-10 fill-current" />
        </a>

        <a
          href="https://www.youtube.com/c/DebbieOBrien"
          target="_blank"
          rel="nofollow noopener noreferrer"
          aria-label="youtube"
        >
          <IconYouTube class="h-10 w-10 fill-current" />
        </a>
        <a
          href="https://www.twitch.tv/debs_obrien"
          target="_blank"
          rel="nofollow noopener noreferrer"
          aria-label="twitch"
        >
          <IconTwitch class="h-10 w-10 fill-current" />
        </a>

        <a
          href="https://github.com/debs-obrien"
          aria-label="github"
          target="_blank"
          rel="nofollow noopener noreferrer"
        >
          <IconGithub class="h-10 w-10 fill-current" />
        </a>

        <a
          href="https://noti.st/debbie"
          aria-label="speaker profile"
          target="_blank"
          rel="nofollow noopener noreferrer"
        >
          <IconSpeaker class="h-10 w-10 fill-current" />
        </a>
        <a
          href="https://www.buymeacoffee.com/debbieobrien"
          aria-label="buy me a coffee"
          target="_blank"
          rel="nofollow noopener noreferrer"
        >
          <IconCoffee class="h-10 w-10 fill-current" />
        </a>
      </div>
      <p class="mt-8 text-center text-base text-gray-800 dark:text-gray-400">
        &copy; Debbie O'Brien, Palma de Mallorca, Spain
      </p>
    </div>
  </footer>
</template>
<script>
  import IconGithub from '@/assets/icons/github.svg?inline'
  import IconTwitter from '@/assets/icons/twitter.svg?inline'
  import IconTwitch from '@/assets/icons/twitch.svg?inline'
  import IconLinkedIn from '@/assets/icons/linkedIn.svg?inline'
  import IconYouTube from '@/assets/icons/youtube.svg?inline'
  import IconSpeaker from '@/assets/icons/speaker.svg?inline'
  import IconCoffee from '@/assets/icons/coffee.svg?inline'
  export default {
    components: {
      IconGithub,
      IconTwitter,
      IconLinkedIn,
      IconYouTube,
      IconSpeaker,
      IconCoffee,
      IconTwitch
    }
  }
</script>

<style scoped></style>

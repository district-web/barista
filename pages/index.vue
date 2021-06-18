<template>
  <div class="gradient leading-relaxed tracking-wide flex flex-col">
    <nav id="header" class="w-full z-30 top-0 text-white py-1 lg:py-6">
      <div
        class="
          w-full
          container
          mx-auto
          flex flex-wrap
          items-center
          justify-between
          mt-0
          px-2
          py-2
          lg:py-6
        "
      >
        <div class="pl-4 flex items-center">
          <a
            class="
              text-white
              no-underline
              hover:no-underline
              font-bold
              text-2xl
              lg:text-4xl
            "
            href="#"
          >
            <img src="~/assets/cup.svg" height="32" width="32" />
            Barista - Caffeine tracker
          </a>
        </div>

        <div class="block lg:hidden pr-4">
          <!--
          <button
            id="nav-toggle"
            class="
              flex
              items-center
              px-3
              py-2
              border
              rounded
              text-gray-500
              border-gray-600
              hover:text-gray-800 hover:border-green-500
              appearance-none
              focus:outline-none
            "
          >
            <svg
              class="fill-current h-3 w-3"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
            </svg>
          </button>-->
        </div>

        <div
          id="nav-content"
          class="
            w-full
            flex-grow
            lg:flex lg:items-center lg:w-auto
            hidden
            lg:block
            mt-2
            lg:mt-0
            text-black
            p-4
            lg:p-0
            z-20
          "
        >
          <!--
          <ul class="list-reset lg:flex justify-end flex-1 items-center">
            <li class="mr-3">
              <a
                class="inline-block py-2 px-4 text-black font-bold no-underline"
                href="#"
                >Active</a
              >
            </li>
            <li class="mr-3">
              <a
                class="
                  inline-block
                  text-black
                  no-underline
                  hover:text-gray-800 hover:text-underline
                  py-2
                  px-4
                "
                href="#"
                >link</a
              >
            </li>
            <li class="mr-3">
              <a
                class="
                  inline-block
                  text-black
                  no-underline
                  hover:text-gray-800 hover:text-underline
                  py-2
                  px-4
                "
                href="#"
                >link</a
              >
            </li>
          </ul>
          <button
            id="navAction"
            class="
              mx-auto
              lg:mx-0
              hover:underline
              text-gray-800
              font-extrabold
              rounded
              mt-4
              lg:mt-0
              py-4
              px-8
              shadow
              opacity-75
            "
          >
            Action
          </button>-->
        </div>
      </div>
    </nav>
    <div class="container mx-auto h-screen">
      <div class="text-center px-3 lg:px-0">
        <h1
          class="my-4 text-2xl md:text-3xl lg:text-5xl font-black leading-tight"
        >
          Start track your caffeine consume
        </h1>
        <p
          class="
            leading-normal
            text-gray-800 text-base
            md:text-xl
            lg:text-2xl
            mb-8
          "
        >
          And learn on your daily impact
        </p>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    }
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen
    },
  },
}
</script>

<style>
@import url('https://rsms.me/inter/inter.css');
html {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto,
    'Helvetica Neue', Arial, 'Noto Sans', sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol', 'Noto Color Emoji';
}

.gradient {
  background-image: linear-gradient(-225deg, #cbbacc 0%, #2580b3 100%);
}

button,
.gradient2 {
  background-color: #f39f86;
  background-image: linear-gradient(315deg, #f39f86 0%, #f9d976 74%);
}

/* Browser mockup code
 * Contribute: https://gist.github.com/jarthod/8719db9fef8deb937f4f
 * Live example: https://updown.io
 */

.browser-mockup {
  border-top: 2em solid rgba(230, 230, 230, 0.7);
  position: relative;
  height: 60vh;
}

.browser-mockup:before {
  display: block;
  position: absolute;
  content: '';
  top: -1.25em;
  left: 1em;
  width: 0.5em;
  height: 0.5em;
  border-radius: 50%;
  background-color: #f44;
  box-shadow: 0 0 0 2px #f44, 1.5em 0 0 2px #9b3, 3em 0 0 2px #fb5;
}

.browser-mockup > * {
  display: block;
}
</style>

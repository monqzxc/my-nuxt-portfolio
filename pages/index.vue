<script setup></script>

<template>
  <!-- <main
      class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 grow items-start w-full"
    >
    
    </main> -->
  <section
    class="flex flex-col md:flex-row mx-auto max-w-7xl px-2 sm:px-6 lg:px-8 grow items-start w-full"
  >
    <div class="py-40 gap-10 flex flex-row justify-between items-center">
      <img
        class="rounded-full shadow-2xl bg-gray-50"
        src="/mon.jpg"
        style="width: 50vh; height: 50vh"
      />

      <div class="flex flex-col">
        <div class="gap-6 flex flex-col p-4 mr-auto">
          <h1 class="text-5xl font-bold uppercase">Hi there!</h1>
          <h1 class="text-5xl font-bold uppercase">
            I'm Anthony <span class="text-yellow-500">Cabigayan</span>
          </h1>

          <p class="font-bold text-fuchsia-500">Back-end Developer</p>
          <div class="flex flex-row gap-2">
            <a target="_blank" href="https://www.linkedin.com/in/monqzxc">
              <img
                class="rounded-full shadow-lg"
                src="/linkedin.png"
                style="width: 25px; height: 25px"
              />
            </a>
            <a target="_blank" href="https://gitlab.com/ancabigayan">
              <img
                class="rounded-full shadow-lg"
                src="/gitlab.png"
                style="width: 25px; height: 25px"
              />
            </a>
            <a target="_blank" href="https://github.com/monqzxc">
              <img
                class="rounded-full shadow-lg"
                src="/github.jpg"
                style="width: 25px; height: 25px"
              />
            </a>
            <a
              target="_blank"
              href="https://profile.codersrank.io/user/monqzxc"
            >
              <img
                class="rounded-full shadow-lg"
                src="/CodersRank.png"
                style="width: 25px; height: 25px"
              />
            </a>
            <a
              target="_blank"
              href="https://www.credly.com/badges/07a81712-0ffb-459b-934c-f68c680caa93/public_url"
            >
              <img
                class="rounded-full shadow-lg"
                src="/credly.png"
                style="width: 25px; height: 25px"
              />
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section></section>
  <!-- <section>
		<h2 class="text-3xl font-bold mt-8">Latest Blog Posts</h2>
		<div class="grid md:grid-cols-3 pt-8 gap-10">
			<Post :posts="posts" />
		</div>
	</section> -->
</template>

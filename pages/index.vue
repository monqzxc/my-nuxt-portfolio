<script setup></script>

<template>
  <section class="flex flex-col md:flex-row">
    <div class="py-40 gap-10 flex flex-row justify-between items-center">
      <img
        class="rounded-full shadow-2xl bg-gray-50"
        src="/resources/images/mon.jpg"
        style="width: 50vh; height: 50vh"
      />

      <div class="flex flex-col">
        <div class="gap-6 flex flex-col p-4 mr-auto">
          <h1 class="text-5xl font-bold uppercase">Hi there!</h1>
          <h1 class="text-5xl font-bold uppercase">
            I'm Anthony <span class="text-yellow-500">Cabigayan</span>
          </h1>

          <p class="font-bold text-fuchsia-500">Back-end Developer</p>
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

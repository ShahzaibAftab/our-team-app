
<script>
import Card from './components/Card.vue';
export default {
    name: 'App',
    components: {
        Card
    }
}
</script>

<template>
<div class=" pt-6 py-6 bg-gray-50 font-inter">
    <h2 class="mx-15 text-2xl text-blue-900"><b>Our Team</b></h2>
    <p class=" mx-15 text-xl mt-2 text-gray-400">Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis.</p>

<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6 mx-15 my-10 ">
  <Card
  image="https://randomuser.me/api/portraits/women/44.jpg"
  name="Emily Johnson"
  title="Creative Designer & Illustrator"
  description="Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis"
  twitter="https://twitter.com/"
  linkedin="https://linkedin.com/in/"
  github="https://github.com/"
/>
  <Card
  image="https://randomuser.me/api/portraits/women/44.jpg"
  name="Emily Johnson"
  title="Creative Designer & Illustrator"
  description="Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis"
  twitter="https://twitter.com/"
  linkedin="https://linkedin.com/in/"
  github="https://github.com/"
/>
  <Card
  image="https://randomuser.me/api/portraits/women/44.jpg"
  name="Emily Johnson"
  title="Creative Designer & Illustrator"
  description="Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis"
  twitter="https://twitter.com/"
  linkedin="https://linkedin.com/in/"
  github="https://github.com/"
/>
  <Card
  image="https://randomuser.me/api/portraits/women/44.jpg"
  name="Emily Johnson"
  title="Creative Designer & Illustrator"
  description="Worem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vulputate libero et velit interdum, ac aliquet odio mattis"
  twitter="https://twitter.com/"
  linkedin="https://linkedin.com/in/"
  github="https://github.com/"
/>

</div>
</div>
</template>

<style>

</style>

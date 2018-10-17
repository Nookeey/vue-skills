<template>
    <div class="about">
        <h1>Hello {{ their_name }}, this is an about page</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Natus aliquid expedita qui quidem, optio nulla mollitia voluptatibus facilis impedit nisi quod veritatis enim? Dolores, non maxime recusandae nisi hic vel?</p>
    </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
        their_name: this.$route.params.name
    }
  }
}
</script>


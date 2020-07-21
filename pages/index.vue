<template>
  <div />
</template>

<script>
export default {
  name: 'Index',
  middleware ({ redirect }) {
    /**
     * this will prevent the generation of the dynamic subpages
     * but the redirect works on first page load of this index file. Which is
     * unexpected!
     */
    redirect(302, '/no/')
  }
}
</script>

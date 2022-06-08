<template>
  <footer class="footer">
    <p class="footer__copy">
      Copyright
    </p>
  </footer>
</template>

<script>
export default {
  name: 'LayoutFooter'
}
</script>

<style lang="scss" scoped>
  .footer {
    height: 40px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #eee;
  }
  .footer__copy {
    font-size: 10px;
    color: #000;
  }
</style>

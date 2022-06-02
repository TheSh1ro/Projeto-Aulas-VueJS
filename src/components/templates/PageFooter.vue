<script>
export default {};
</script>
<template>
  <footer id="footer">
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
    <div class="footer-social">
      <span class="social-item">Instagram</span>
      <span class="social-item">Twitter</span>
    </div>
  </footer>
</template>
<style scoped>
#footer {
  grid-area: footer;
  display: flex;
  flex-direction: row;
  align-items: stretch;
  justify-content: space-evenly;
  padding: 5px;

  background-color: rgb(50, 80, 160);
  font-size: 1.2em;
}
.footer-social {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-evenly;
}
.social-item {
  border-bottom: 2px ridge black;
  cursor: pointer;
}
.social-item:hover {
  color: rgb(30, 30, 30);
  border-bottom: 2px ridge darkred;
}
</style>

 <template>
  <div>
    <footer class="page-footer text-center ml-3">
          <a href="https://github.com/Ahmet-Kirmizi"><font-awesome-icon :icon="['fab', 'github']" class="fa-lg m-2 text-light" /></a>
          <a href="https://twitter.com/_ahmetk5113_"><font-awesome-icon :icon="['fab', 'twitter']" class="fa-lg m-2 text-light" /></a>
          <a href="https://www.linkedin.com/in/ahmet-kirmizi-00962920b/"><font-awesome-icon :icon="['fab', 'linkedin']" class="fa-lg m-2 text-light" /></a>
          <h6>&copy; Copyright 2021 Ahmet Kırmızı</h6>

    </footer>
  </div>
</template>
<script>

export default{
    name : "footerbar"
}
</script>
<style scoped>
@media only screen and (max-width: 993px) {
h6{
  font-size: 15px;
}
}
/*
footer.page-footer.text-center{
  color: #ffff ;
}
*/
</style>
 

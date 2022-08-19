    <template>
  <div>
    <nav class="navbar navbar-expand-lg navbar-dark navbarMain mt-1">
      <div class="container-fluid">
        <div class="navbar-nav">
          <router-link class="nav-link activetext" aria-current="page" to="/"
            >HOME</router-link
          >
          <div class="navbarBlog ml-3">
            <router-link class="nav-link navbarlinks" to="/blog"
              >BLOG</router-link
            >
          </div>
          <div class="ml-3">
            <router-link class="nav-link navbarlinks" to="/about"
              >ABOUT</router-link
            >
          </div>
          <div class="ml-3">
            <router-link class="nav-link navbarlinks" to="/portfolio"
              >PORTFOLIO</router-link
            >
          </div>
        </div>
        <div class="float-right nav-icons ">
          <a href="https://github.com/Ahmet-Kirmizi"
            ><font-awesome-icon
              :icon="['fab', 'github']"
              class="fa-lg m-2 text-light"
          /></a>
          <a href="https://twitter.com/_ahmetk5113_"
            ><font-awesome-icon
              :icon="['fab', 'twitter']"
              class="fa-lg m-2 text-light"
          /></a>
          <a href="https://www.linkedin.com/in/ahmet-kirmizi-00962920b/"
            ><font-awesome-icon
              :icon="['fab', 'linkedin']"
              class="fa-lg m-2 text-light"
          /></a>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="18"
            height="18"
            fill="currentColor"
            class="bi bi-lightbulb mb-4 ml-4"
            viewBox="0 0 16 16"
            v-on:click="darkMode()"
          >
            <path
              d="M2 6a6 6 0 1 1 10.174 4.31c-.203.196-.359.4-.453.619l-.762 1.769A.5.5 0 0 1 10.5 13a.5.5 0 0 1 0 1 .5.5 0 0 1 0 1l-.224.447a1 1 0 0 1-.894.553H6.618a1 1 0 0 1-.894-.553L5.5 15a.5.5 0 0 1 0-1 .5.5 0 0 1 0-1 .5.5 0 0 1-.46-.302l-.761-1.77a1.964 1.964 0 0 0-.453-.618A5.984 5.984 0 0 1 2 6zm6-5a5 5 0 0 0-3.479 8.592c.263.254.514.564.676.941L5.83 12h4.342l.632-1.467c.162-.377.413-.687.676-.941A5 5 0 0 0 8 1z"
            />
          </svg>
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="18"
            height="18"
            fill="currentColor"
            class="bi bi-lightbulb-fill mb-4 ml-3 whitebulb"
            viewBox="0 0 16 16"
            v-on:click="lightMode()"
          >
            <path
              d="M2 6a6 6 0 1 1 10.174 4.31c-.203.196-.359.4-.453.619l-.762 1.769A.5.5 0 0 1 10.5 13h-5a.5.5 0 0 1-.46-.302l-.761-1.77a1.964 1.964 0 0 0-.453-.618A5.984 5.984 0 0 1 2 6zm3 8.5a.5.5 0 0 1 .5-.5h5a.5.5 0 0 1 0 1l-.224.447a1 1 0 0 1-.894.553H6.618a1 1 0 0 1-.894-.553L5.5 15a.5.5 0 0 1-.5-.5z"
            />
          </svg>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "navbarTop",
  methods: {
    lightMode: function () {
      document
        .querySelector("body")
        .setAttribute("style", "background:#8AACB7");
      
        document.getElementsByTagName("h6")[1].setAttribute("style", "color:	#FFFFFF");
        document.getElementsByTagName("h6")[2].setAttribute("style", "color:	#FFFFFF");
        document.getElementsByTagName("h6")[3].setAttribute("style", "color:	#FFFFFF");
        document.getElementsByTagName("h6")[4].setAttribute("style", "color:	#FFFFFF");
        document.getElementsByTagName("h6")[5].setAttribute("style", "color:	#FFFFFF");

},
    darkMode: function () {
      document
        .querySelector("body")
        .setAttribute("style", "background:#1a202c");
    },
  },
};
</script>
<style scoped>
.whitebulb{
  color: rgb(255, 255, 255);
}
a{
  font-size: 1em;
  color: white !important;
}
@media only screen and (max-width: 993px) {
  div.navbar-nav {
    flex-direction: row;
  }
  div.float-right.nav-icons {
    display: none;
  }
  .navbar-nav a.activetext {
    border-bottom: 1px solid #1a202c;
  }

}
</style>
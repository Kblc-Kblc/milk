<template>
  <div class="home">
    <NavBar />
    <Searchbar />
    <Navigation />
    <ContentOne />
    <ContentRoom />
    <ButtonMore />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/Navbar";
import Searchbar from "@/components/Searchbar";
import Navigation from "@/components/Navigation";
import ContentOne from "@/components/Content-one";
import ContentRoom from "@/components/Content-room";
import ButtonMore from "@/components/Button-more";
import Footer from "@/components/Footer";

export default {
  name: "Home",
  components: {
    NavBar,
    Searchbar,
    Navigation,
    ContentOne,
    ContentRoom,
    ButtonMore,
    Footer,
  },
};
</script>

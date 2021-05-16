<template>
  <div class="container">
    <Header/>
    <Slide/>
    <Logos/>
    <Content/>
    <Map/>
    <Metrika/>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Map from "@/components/Map";
import Slide from "@/components/Slide";
import Content from "@/components/Content";
import Logos from "@/components/Logos";
import Metrika from "@/components/Metrika";

export default {
  name: 'App',
  components: {
    Metrika,
    Logos,
    Content,
    Slide,
    Map,
    Header
  }
}
</script>

<style>
@import "./assets/css/layout.css";
</style>

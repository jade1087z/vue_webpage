<script setup>
  import Header from "@/components/Header.vue"
  import Footer from "@/components/Footer.vue"
  import Slider from "@/components/Slider.vue"
  import Image from "@/components/Image.vue"
  import ImageText from "@/components/ImageText.vue"
  import Card from "@/components/Card.vue"
  import Banner from "@/components/Banner.vue"
  import Text from "@/components/Text.vue"
</script>

<template>

  <Header element="nexon" />
  <main>
    <Slider Element="nexon" title="슬라이드" span="DEVELOPER"/>
    <Image Element="section nexon" h2="포트폴리오가 실력이다."/> 
    <ImageText Element="section nexon"/>
    <Card Element="section nexon" />
    <Banner Element="nexon"/>
    <Text Element="nexon section"/>
  </main>
  <Footer Element="nexon section"/>

</template>

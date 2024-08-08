<script setup>
import { footerData } from "./footerData";
</script>

<template>
  <footer class="footer container">
    <div class="footer_head">
      <Logo :size="24" variant="white" />
      <Navigation variant="white" />
      <div class="footer_header_social_media">
        <a v-for="item in footerData.socialmedia" href="">
          <img :src="item" alt="Иконка соц. сети" />
        </a>
      </div>
    </div>
    <div class="footer_content">
      <div class="contact_us">
        <h4>{{ footerData.title }}</h4>
        <p>{{ footerData.email }}</p>
        <p>{{ footerData.phone }}</p>
        <p>{{ footerData.address }}</p>
      </div>
      <div class="subscribe_form">
        <input type="text" name="" id="" placeholder="Email" />
        <button class="btn">{{ footerData.button.title }}</button>
      </div>
    </div>
    <div class="copyright">
      <hr />
      <div>
        <p>{{ footerData.copyrigth }}</p>
        <a href="">{{ footerData.documentslink.title }}</a>
      </div>
    </div>
  </footer>
</template>

<style lang="scss"></style>

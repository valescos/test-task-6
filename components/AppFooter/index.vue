<script setup>
import { footerData } from "./footerData";
</script>

<template>
  <footer class="footer container">
    <div>
      <Logo :size="24" variant="white" />
      <Navigation variant="white" />
      <img
        v-for="item in footerData.socialmedia"
        :src="item"
        alt="Иконка соц. сети"
      />
    </div>
    <div class="footer_wrapper">
      <div class="contact_us">
        <h4>{{ footerData.title }}</h4>
        <p>{{ footerData.email }}</p>
        <p>{{ footerData.phone }}</p>
        <p>{{ footerData.address }}</p>
      </div>
      <div class="subscribe_form">
        <input type="text" name="" id="" placeholder="Email" />
        <button>{{ footerData.button.title }}</button>
      </div>
    </div>
    <hr />
    <div class="copyright">
      <p>{{ footerData.copyrigth }}</p>
      <a href="">{{ footerData.documentslink.title }}</a>
    </div>
  </footer>
</template>

<style lang="scss"></style>

<template>
  <div id="app">
    <BaseHeader @show-sidebar="handleSidebar" />
    <router-view />
    <BaseFooter :showSideBar="isShowSideBar" />
  </div>
  <Chatbot/>
</template>

<script>
import BaseHeader from './components/BaseHeader'
import BaseFooter from './components/BaseFooter'
import Chatbot from './components/Chatbot'
// import user from '@/modules/user/store'
// import products from '@/modules/product/store'
export default {
  data: () => ({
    isShowSideBar: false
  }),

  components: {
    BaseHeader,
    BaseFooter,
    Chatbot
  },

  methods: {
    handleSidebar(showSideBar) {
      this.isShowSideBar = showSideBar
    }
  },

  created() {
    // if (! this.$store.hasModule('userName')) {
    // this.$store.registerModule('userName', user)
    // }
    // if (! this.$store.hasModule('products')) {
    // this.$store.registerModule('products', products)
    // }
  }
}
</script>

<style></style>

<template>
  <div>
    <!-- <app-header v-bind:프롭스 속성 이름="상위 컴포넌트의 데이터 이름"></app-header> -->
    <app-header v-bind:propsdata="str" v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {

  data() {
    return {
      str: 'Header'
    };
  },

  mounted() {
    
  },

  methods: {
    renewStr: function(){
      this.str = 'hi';
    }
  },

  components: {
    'app-header': AppHeader
  }
};
</script>

<style>

</style>
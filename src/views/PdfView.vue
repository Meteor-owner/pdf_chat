<template>
    <div class="container">
      <button @click="openpdf">打开pdf</button>
      <vueshowpdf @closepdf="closepdf"
                  v-model="isshowpdf"
                  :pdfurl="src"
                  @pdferr="pdferr"
                  :maxscale='4'
                  :minscale='0.6'
                  :scale='1.0'></vueshowpdf>
    </div>
  </template>
  
  <script>
  import vueshowpdf from 'vueshowpdf'
  export default {
    components: {
      vueshowpdf
    },
    data () {
      return {
        src: 'D:/Graduation Project/Design and Implementation of a Big Data-based Rental Recommendation System.pdf',
        isshowpdf: false
      }
    },
    methods: {
      closepdf () {
        this.isshowpdf = false
      },
      pdferr (errurl) {
        console.log(errurl)
      },
      openpdf () {
        this.isshowpdf = true
      }
    }
  }
  </script>
  
  <style scoped>
  .container {
    font-family: PingFang SC;
    width: 100%;
  }
  </style>
  
  
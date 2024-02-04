<template>
    <!-- <iframe :src="pageUrl" frameborder="0" style="width: 100%; height: 100%"></iframe> -->
    <iframe id="myframe"
    src="https://www.tandfonline.com/doi/epdf/10.1080/13658816.2015.1086924"
      width="100%" height="1000" frameborder="0"></iframe>
  </template>
    
  <script>
  export default {
    props: {
      pageUrl: {
        // 嵌入页面URL
        type: String,
        default: "",
      },
    },
    data() {
      return {};
    },
    methods: {},
  };
  </script>
    
  <style lang="scss" scoped>
  </style>
  
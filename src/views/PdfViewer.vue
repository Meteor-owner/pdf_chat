<template>
  <div class="pdf-viewer">
    <object :data="pdfUrl" type="application/pdf" width="100%" height="600">
      <p>您的浏览器不支持PDF嵌入。<a :href="pdfUrl">点击这里下载PDF文件</a>。</p>
    </object>
  </div>
</template>
  
<script>
export default {
  name: 'PdfViewer',
  props: {
    pdfUrl: {
      type: String,
      required: true
    }
  }
}
</script>
  
<style>
.pdf-viewer {
 width: 100%;
}
</style>
  
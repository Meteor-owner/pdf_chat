<template>
  <div class="header">
    <header>
      <div class="header-container">
        <div class="nav-link">
          <ul class="fll">
            <router-link to="/">
              <li>首页</li>
            </router-link>
            <router-link to="/houseList">
              <li>房源</li>
            </router-link>
            <router-link to="/offer">
              <li>发布房源</li>
            </router-link>
            <router-link to="/userPage">
              <li>个人中心</li>
            </router-link>
          </ul>
        </div>
        
      </div>
    </header>
  </div>
</template>

<script>

export default {
  name: 'HomeView',
  components: {
  }
}
</script>


<style scoped>
.ul{
list-style: none;
}
</style>
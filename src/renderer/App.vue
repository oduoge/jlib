<template>
  <div id="app" class="main">
    <div class="sider-bar">
      <j-sidebar />
    </div>
    <div class="body-frame">
      <div class="header">
        <j-header />
      </div>

      <div class="content">
        aa
      </div>
    </div>
  </div>
</template>

<script>
  import JSidebar from '@/components/JSidebar'
  import JInfobar from '@/components/JInfobar'
  import JHeader from '@/components/JHeader'
  export default {
    components: {
      JSidebar,
      JInfobar,
      JHeader,
    },
    name: 'jlib'
  }
</script>

<style scoped>
.main {
  display: flex;
  flex-direction: row;
}
.sider-bar {
  background: red;
  float: left;
  width: 220px;
  height: 100vh;
}

.body-frame {
  background: green;
  width: 100%;
  height: 100vh;
}

.body-frame .header {
  background: gray;
  height: 32px;
  text-align: right;
  -webkit-app-region: drag;
}

.body-frame .content {
  background: yellow;
  height: calc(100vh - 32px);
}
</style>

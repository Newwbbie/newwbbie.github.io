<template>
  <div id="main" :style="{height: height}">
    <div class="space" />
    <div id="center" style="border-radius: 5px;">
      <n-scrollbar>
        <div id="card-parent" :style="{width: '1000px', height: height}">
          <div class="flex1">
            <div class="flex1 padding4">
              <n-card title="卡片1" hoverable>
                卡片内容
              </n-card>
            </div>
            <div class="flex2 padding4">
              <n-card title="卡片2" hoverable>
                卡片内容
              </n-card>
            </div>
          </div>
          <div class="flex2">
            <div class="flex1 padding4">
              <n-card title="卡片3" hoverable>
                卡片内容
              </n-card>
            </div>
            <div class="flex1 padding4">
              <n-card title="卡片4" hoverable>
                卡片内容
              </n-card>
            </div>
          </div>
        </div>

      </n-scrollbar>
    </div>
    <div class="space" />
  </div>
</template>

<script>

export default {
  data() {
    return {
      height: ''
    }
  },
  created() {
  },
  computed: {
    height: function () {
      return window.innerHeight - 20 + 'px'
    }
  },
  methods: {
  }
}
</script>

<style scoped>
#main {
  width: 100%;
  height: 100%;
  display: flex;
}
.space {
  flex: 1;
}
#center {
  max-width: 1000px;
  /*background: antiquewhite;*/
}
#card-parent {
  width: 100%;
  height: 100%;
  display: flex;
  max-width: 1000px;
}
.flex1 {
  flex: 1;
}
.flex2 {
  flex: 2;
}
.padding4 {
  padding: 4px;
}
</style>

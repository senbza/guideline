<template>
  <div>
    <h1>开着网页即可。每30秒清空一下内存</h1>
    <el-button @click="kaiqi">开启清除内存</el-button>
    <el-button @click="guanbi">关闭清除内存</el-button>
    <div class="neicun">
      <p class="heise" v-for="item in shuzu">成功释放内存:{{ item.neicunshuliang }}mb</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      shuzu: [],
      timer: null
    }
  },
  methods: {
    kaiqi() {
      this.timer = setInterval(() => {
        this.shuzu.push({
          neicunshuliang: Math.floor(Math.random() * 200 + 1)
        })
      }, 30000);
    },
    guanbi() {
      clearInterval(this.timer);
      this.timer = null;
      this.shuzu = []

    }
  }
}
</script>

<style scoped>
.neicun {
  height: 600px;
  background: #000;
  overflow: scroll
}

.heise {
  color: #fff
}
</style>
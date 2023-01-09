<template>
  <h3>爆肝攻略——贡献者鱼鞭</h3>
  <h3>新人小知识</h3>
  <p>新来的同学可以在群里联系一下幕后老板。（ps:自己一定要有100点活跃哦）<span style="color:blue">联系群里幕后煮屎人</span>如果幕后老板有空可以带一下你。四个号可以弄20亿+金钱，几十亿经验。
  </p>
  <h3>广告招牌</h3>
  <p>群里<span style="color:blue">@木之本樱、@1119、@妈妈桑、@唐长老</span>如果你有修炼果，可以换任何游戏资源，如有需要请在群里@他们</p>
  <h2>新人小福利</h2>
  <p>五个号69以后，可以在群里<span style="color:blue">@木之本樱、@1119、@妈妈桑、@唐长老、@幕后煮屎人</span>领取新人路费。一头秒10的神兽鲲，和50万仙玉作为起步资金</p>
  <el-tabs class="tabs" v-model="activeName" type="border-card" @tab-click="handleClick">
    <el-tab-pane label="版本介绍" name="first">
      <gonglue />
    </el-tab-pane>
    <el-tab-pane label="新人攻略" name="first2">
      <gonglue1></gonglue1>
    </el-tab-pane>
    <el-tab-pane label="每日必做" name="second">
      <bizuo></bizuo>
    </el-tab-pane>
    <el-tab-pane label="材料介绍" name="fourth">
      <cailiao></cailiao>
    </el-tab-pane>
    <el-tab-pane label="怪物爆率" name="baolv">
      <guaiwu></guaiwu>
    </el-tab-pane>
    <el-tab-pane label="跑环介绍" name="bao">
      <paohuan></paohuan>
    </el-tab-pane>
    <el-tab-pane label="人物神器法宝" name="th3i32rd">
      <h1>【法宝神器灵宝篇】</h1>
      法宝不卖、只能游戏活动直接爆法宝或者抽奖盒子抽出法宝也可以法宝任务书做任务得到法宝；材料合法宝和加灵气在天宫30.150太上老君处。。。神器去天台袁天罡处领取神器任务完成后获得神器。。。灵宝可在天宫30.150太上老君处领取任务完成后可获得一个灵宝，也可以在这用银子买更多灵宝，以上神器和灵宝任务有一定难度可喊人帮杀
      <img src="./assets/QQ20230103-35.jpg" alt="" />
    </el-tab-pane>
    <el-tab-pane label="人物神器技能介绍" name="third">
      <img src="./assets/QQ20230103-32.png" alt="" />
    </el-tab-pane>
    <el-tab-pane label="灵饰特效套装" name="th3ird">
      <img style="width:1200px;height:900px" src="./assets/QQ20230103-33.png" alt="" />
    </el-tab-pane>
    <el-tab-pane label="神兽培养图" name="th3i2rd">
      <img src="./assets/QQ20230103-34.jpg" alt="" />
    </el-tab-pane>
    <el-tab-pane label="内存清理" name="th33i2rd">
      <neicun></neicun>
    </el-tab-pane>
  </el-tabs>
</template>

<script>
import gonglue from './components/gonglue.vue'
import gonglue1 from './components/gonglue1.vue'
import bizuo from './components/bizuo.vue'
import cailiao from './components/cailiao.vue'
import guaiwu from './components/guaiwu.vue'
import paohuan from './components/paohuan.vue'
import neicun from './components/neicun.vue'

export default {
  name: 'App',
  components: {
    gonglue,
    gonglue1,
    bizuo,
    cailiao,
    guaiwu,
    paohuan,
    neicun
  },
  data() {
    return {
      activeName: 'first2'
    }
  }
}
</script>

<style>
#app {
  margin: 0;
  padding: 0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

/* .tabs {
  display: flex;
  justify-content: space-around;
  flex-direction: column;
} */

.el-tabs__nav-scroll {
  display: flex;
  justify-content: space-around;
  flex-direction: column;
}
</style>

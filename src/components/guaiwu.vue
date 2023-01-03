<template>
  <div>
    <h2>在游戏内点击梦幻精灵即可看到爆率，下面的地址点了直接飞过去。需要10w银两。此处的爆率是在上面没有的。</h2>
    <img style="width:500px;height:300px" src="../assets/QQ20230103-31.png" alt="" />
    <h2>下面的爆率是你有一定实力后去挑战，如果没刷怪物的话，打打知了，神器地煞即可。全图都是</h2>
    <el-table :data="tableData" border style="width: 100%">
      <el-table-column prop="name" label="怪物名称">
      </el-table-column>
      <el-table-column prop="nandu" label="怪物难度">
      </el-table-column>
      <el-table-column prop="didian" label="刷新地点">
      </el-table-column>
      <el-table-column prop="shijian" label="刷新时间">
      </el-table-column>
      <el-table-column prop="diaoluo" label="怪物掉落">
      </el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tableData: [{
        name: '梁山好汉',
        nandu: '需要满魂环3鲲',
        shijian: '每小时15分',
        didian: '大雁塔1-6',
        diaoluo: '转生材料，九转金丹'
      }, {
        name: '实力质检员',
        nandu: '需要满魂环1速北冥+4鲲',
        shijian: '每小时10分',
        didian: '朱紫国、长寿村',
        diaoluo: '修炼果10个、七彩石、装备升星石等'
      }, {
        name: '魔童降世',
        nandu: '需要能打200W左右的时候再去挑战',
        shijian: '每小时20分',
        didian: '东海岩洞',
        diaoluo: '超级多。没打过不知道。'
      }, {
        name: '卢雨寒',
        nandu: '需要满魂环1速北冥+4鲲',
        shijian: '每小时06分',
        didian: '东海岩洞',
        diaoluo: '400活动积分、幽魂之水、足迹升级、锦衣升级、光环升级'
      }]
    }
  }
}
</script>

<style>

</style>
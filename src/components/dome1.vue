<template>
  <div class="hello">
    <mt-header title="销售KPI">
      <mt-button icon="close" slot="left"></mt-button>
      <mt-button icon="more" slot="right"></mt-button>
    </mt-header>

    <div>
      <mt-navbar v-model="view.timeType">
        <mt-tab-item v-for="(item, index) in metadata.timeTypeList" :key="index" :id="item.key">{{item.name}}</mt-tab-item>
      </mt-navbar>
    </div>

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      view: {
        timeType: 5
      },
      metadata: {
        timeTypeList: [
          {
            key: 1,
            name: '昨日'
          },
          {
            key: 2,
            name: '上周'
          },
          {
            key: 3,
            name: '本周'
          },
          {
            key: 4,
            name: '上月'
          },
          {
            key: 5,
            name: '本月'
          },
          {
            key: 6,
            name: '年至今'
          }
        ]
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">

</style>

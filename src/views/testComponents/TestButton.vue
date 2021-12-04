<!--
  功能：功能描述
  作者：wp
  邮箱：wu_pan123@126.com
  时间：2021年11月22日 08:00:29
  版本：v1.0
  修改记录：
  修改内容：
  修改人员：
  修改时间：
-->
<template>
  <page-header-wrapper>
    <div class="test-grid" id="test-grid">
      <a-row
        type="flex"
        justify="end"
        align="middle"
        :gutter="[
          { xs: 8, sm: 16, md: 16, lg: 16 },
          { xs: 8, sm: 16, md: 16, lg: 16 }
        ]"
      ><!--  gutter推荐使用 (16+8n)px,gutter数组形式 [水平间距, 垂直间距] -->
        <a-col :span="24" :offset="0" :order="1">
          <a-row
            type="flex"
            justify="space-between"
            align="middle"
            :gutter="[
              { xs: 8, sm: 8, md: 8, lg: 8 },
              { xs: 8, sm: 8, md: 8, lg: 8 }
            ]"
          ><!--  gutter推荐使用 (16+8n)px,gutter数组形式 [水平间距, 垂直间距] -->
            <a-col :span="auto" :offset="0">
              <a-button type="primary" shape="circle">
                <template #icon><!-- <WifiOutlined /> --></template></a-button
              ></a-col
            >
          </a-row>
        </a-col>
        <a-col :span="24" :offset="0" :order="1">
          <a-row
            type="flex"
            justify="space-between"
            align="middle"
            :gutter="[
              { xs: 8, sm: 8, md: 8, lg: 8 },
              { xs: 8, sm: 8, md: 8, lg: 8 }
            ]"
          ><!--  gutter推荐使用 (16+8n)px,gutter数组形式 [水平间距, 垂直间距] -->
            <a-col :span="4" :offset="0" :order="1"><div style="background: #000; color: #fff">content</div></a-col>
            <a-col :span="4" :offset="0" :order="2">content</a-col>
            <a-col :flex="1" :offset="0" :order="4"><div style="background: #000; color: #fff">content</div></a-col>
            <a-col :flex="2" :offset="0" :order="5"><div style="background: red; color: #fff">content</div></a-col>
            <a-col flex="100px" :offset="0" :order="6"><div style="background: blue; color: #fff">content</div></a-col>
            <a-col flex="auto" :offset="0" :order="7"><div style="background: yellow; color: #fff">content</div></a-col>
            <a-col
              :xs="{ span: 1, offset: 0, order: 8 }"
              :sm="{ span: 1, offset: 0, order: 8 }"
              :md="{ span: 1, offset: 0, order: 8 }"
              :lg="{ span: 1, offset: 0, order: 8 }"
              :xl="{ span: 1, offset: 0, order: 8 }"
              :xxl="{ span: 1, offset: 0, order: 8 }"
            >cintent</a-col
            >
          </a-row>
        </a-col>
        <a-col :span="24" :offset="0" :order="1">
          <a-row type="flex" justify="end">
            <a-col :span="auto" :offset="0" :order="1"> <a-button type="primary">这是一个测试按钮</a-button></a-col>
          </a-row></a-col
        >
      </a-row>
    </div>
  </page-header-wrapper>
</template>
<script>
// @ is an alias to /src
// import Test from "@/components/Test.vue";
/* import { WifiOutlined } from '@ant-design/icons-vue' */
export default {
  // 组件名称
  name: 'TestButton',
  // 组件参数 接收来自父组件的数据
  props: {},
  // 局部注册的组件
  components: {
    /*  WifiOutlined: WifiOutlined */
  },
  // 组件状态值
  data () {
    return {}
  },
  // 计算属性
  computed: {},
  // 侦听器
  watch: {},
  // 组件方法
  methods: {},
  // 以下是生命周期钩子   注：没用到的钩子请自行删除
  /**
   * 在实例初始化之后，组件属性计算之前，如data属性等
   */
  beforeCreate () {},
  /**
   * 组件实例创建完成，属性已绑定，但DOM还未生成，$ el属性还不存在
   */
  created () {},
  /**
   * 在挂载开始之前被调用：相关的 render 函数首次被调用。
   */
  beforeMount () {},
  /**
   * el 被新创建的 vm.$ el 替换，并挂载到实例上去之后调用该钩子。
   * 如果 root 实例挂载了一个文档内元素，当 mounted 被调用时 vm.$ el 也在文档内。
   */
  mounted () {},
  /**
   * 数据更新时调用，发生在虚拟 DOM 重新渲染和打补丁之前。
   * 你可以在这个钩子中进一步地更改状态，这不会触发附加的重渲染过程。
   */
  beforeUpdate () {},
  /**
   * 由于数据更改导致的虚拟 DOM 重新渲染和打补丁，在这之后会调用该钩子。
   * 当这个钩子被调用时，组件 DOM 已经更新，所以你现在可以执行依赖于 DOM 的操作。
   */
  updated () {},
  /**
   * keep-alive 组件激活时调用。 仅针对keep-alive 组件有效
   */
  activated () {},
  /**
   * keep-alive 组件停用时调用。 仅针对keep-alive 组件有效
   */
  deactivated () {},
  /**
   * 实例销毁之前调用。在这一步，实例仍然完全可用。
   */
  beforeUnmount () {},
  /**
   * Vue 实例销毁后调用。调用后，Vue 实例指示的所有东西都会解绑定，
   * 所有的事件监听器会被移除，所有的子实例也会被销毁。
   */
  unmounted () {}
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<!--使用了scoped属性之后，父组件的style样式将不会渗透到子组件中，-->
<!--然而子组件的根节点元素会同时被设置了scoped的父css样式和设置了scoped的子css样式影响，-->
<!--这么设计的目的是父组件可以对子组件根元素进行布局。-->
<style lang="less" scoped>
#components-grid-demo-flex :deep(.a-row) {
  background: rgba(128, 128, 128, 0.08);
}
</style>

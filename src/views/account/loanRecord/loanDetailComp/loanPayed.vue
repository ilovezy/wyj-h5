<template>
  <div>
    <interest-modal :show='showIntroModal'
                    :close='closeIntroModal'/>

    <div class='simple-panel'>
      <div class='panel-title'>出借信息详情</div>
      <div class='data-wrap'>
        <button class='btn-tiny-blue'>复制</button>
        <div class='data-item'>出借订单号：xxxxxx</div>
        <div class='data-item'>标的名称：<span class='text-info'>车新宝284号</span></div>
        <div class='data-item'>标的期限：90天</div>
        <div class='data-item'>标的利率：8.0%</div>
        <div class='data-item'>还款方式：按月付息，到期还本付息</div>
        <div class='data-item'>出借金额：3,000元</div>
        <div class='data-item'>出借时间：2017/07/12 13:23:22</div>
        <div class='data-item'>预期利息：66元
          <span class='icon icon-group40'
                @click='openIntroModal'></span>
        </div>
        <div class='data-item'>标的状态：已还款</div>
        <div class='data-item'>借款协议：<span class='text-info'>《出借协议》</span></div>
      </div>
    </div>

    <div class='simple-panel'>
      <div class='panel-title'>还款计划表</div>

      <div class='plan-wrap'>
        <div class='plan-item'>
          <div class='data-info'>
            <div class='left'>还款时间：2017/07/12</div>
            <div class='right'>已还款</div>
          </div>
          <div class='data-info'>
            <div class='left'>还款金额：22元</div>
          </div>
          <div class='data-info'>
            <div class='left'>本金：0元</div>
            <div class='right'>利息：22元</div>
          </div>
        </div>
        <div class='plan-item'>
          <div class='data-info'>
            <div class='left'>还款时间：2017/07/12</div>
            <div class='right'>已还款</div>
          </div>
          <div class='data-info'>
            <div class='left'>还款金额：22元</div>
          </div>
          <div class='data-info'>
            <div class='left'>本金：0元</div>
            <div class='right'>利息：22元</div>
          </div>
        </div>
        <div class='plan-item'>
          <div class='data-info'>
            <div class='left'>还款时间：2017/07/12</div>
            <div class='right'>已还款</div>
          </div>
          <div class='data-info'>
            <div class='left'>还款金额：22元</div>
          </div>
          <div class='data-info'>
            <div class='left'>本金：0元</div>
            <div class='right'>利息：22元</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>

  export default {

    data() {
      return {
        showModal: false,
        showIntroModal: false
      }
    },
    created() {
    },

    methods: {
      doCopy() {
        alert('fuck')
      },
      openIntroModal() {
        this.showIntroModal = true
      },
      closeIntroModal() {
        this.showIntroModal = false
      },
      openModal() {
        this.showModal = true
      },
      closeModal() {
        this.showModal = false
      }
    }
  }
</script>

<script lang="ts" setup>
import topEnterpriseTrial from '@/assets/svg/top-enterprise-trial.svg'
import topHelpDoc from '@/assets/svg/top-help-doc.svg'
import topProductBbs from '@/assets/svg/top-product-bbs.svg'
import topTechnology from '@/assets/svg/top-technology.svg'
import docs from '@/assets/svg/docs.svg'
import { computed } from 'vue'
import { Icon } from '@/components/icon-custom'
import TopDocCard from '@/layout/components/TopDocCard.vue'
import { useAppearanceStoreWithOut } from '@/store/modules/appearance'
const appearanceStore = useAppearanceStoreWithOut()
const navigateBg = computed(() => appearanceStore.getNavigateBg)
const help = computed(() => appearanceStore.getHelp)

const cardInfoList = [
  { name: '帮助文档', url: help.value || 'https://dataease.io/docs/v2/', icon: topHelpDoc },
  { name: '产品论坛', url: 'https://bbs.fit2cloud.com/c/de/6', icon: topProductBbs },
  {
    name: '技术博客',
    url: 'https://blog.fit2cloud.com/categories/dataease',
    icon: topTechnology
  },
  { name: '企业版试用', url: 'https://jinshuju.net/f/TK5TTd', icon: topEnterpriseTrial }
]
</script>

<template>
  <el-popover
    :show-arrow="false"
    popper-class="top-popover"
    placement="bottom-end"
    width="210"
    trigger="hover"
  >
    <top-doc-card
      :span="12"
      v-for="(item, index) in cardInfoList"
      :key="index"
      :card-info="item"
    ></top-doc-card>
    <template #reference>
      <div
        class="sys-setting"
        :class="{ 'is-light-setting': navigateBg && navigateBg === 'light' }"
      >
        <el-icon>
          <Icon name="docs"><docs class="svg-icon" /></Icon>
        </el-icon>
      </div>
    </template>
  </el-popover>
</template>

<style lang="less" scoped>
.sys-setting {
  margin: 0 10px;
  padding: 5px;
  height: 28px;
  width: 28px;
  border-radius: 4px;
  overflow: hidden;
  cursor: pointer;
  &:hover {
    background-color: #1e2738;
  }
}
.is-light-setting {
  &:hover {
    background-color: #1f23291a !important;
  }
}
</style>

<style lang="less">
.top-popover {
  display: flex;
  padding: 8px !important;
  flex-wrap: wrap;
  .doc-card {
    margin: auto;
  }
}
</style>

<template>
  <div>
    <page-title label="ABOUT" />
    <div class="about__cont">
      <ul class="about__list">
        <li
          v-for="(item, index) in items"
          :key="`item-${index}`"
          class="about__listItem"
        >
          <p class="about__listLabel">
            {{ item.label }}
          </p>
          <p class="about__listValue">
            {{ item.value }}
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
import HeaderMeta from '~/mixins/meta'
export default {
  name: 'AboutPage',
  mixins: [HeaderMeta],
  data () {
    return {
      items: [
        {
          label: '会社名',
          value: 'Sample-Corp'
        },
        {
          label: '所在地',
          value: '日本'
        },
        {
          label: '設立',
          value: '2022年3月'
        },
        {
          label: '事業内容',
          value: '〇〇〇〇〇〇〇'
        },
        {
          label: '代表者名',
          value: '〇〇　〇〇'
        }
      ],
      meta: {
        title: '会社情報',
        description: 'aboutのdescription',
        ogUrl: 'https://example.com/about/'
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.about__cont {
  width: 100%;
}
.about__list {
  width: 100%;
}
.about__listItem {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  border-bottom: 1px solid #707070;
  padding: 25px 15px;
  &:first-of-type {
    border-top: 1px solid #707070;
  }
}
.about__listLabel {
  max-width: 200px;
  width: 100%;
  font-size: 16px;
  font-weight: 600;
  color: #333;
}
.about__listValue {
  font-size: 15px;
  font-weight: 300;
  color: #333;
}
</style>

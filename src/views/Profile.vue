<template>
  <div class="Profile">
    <h1>Profile</h1>
    <div class="texts">
      <text-box v-for="text in texts" :key="text.title" :item="text" />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import TextBox from '@/components/TextBox.vue'

export default {
  name: 'Profile',
  components: {
    TextBox
  },
  data () {
    return {
      texts: [
        {
          title: '名前',
          content: '内藤 佑馬(ないとう ゆうま)'
        },
        {
          title: '大学',
          content: '北海学園大学 経営情報学科 3年'
        },
        {
          title: '経歴',
          content: `サンプルテキスト
                    サンプルテキストああああ
                    ああああああああああああ
                    ああああああああああああ
                    ああああああ`
        }
      ]
    }
  }
}
</script>

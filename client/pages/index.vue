<template>
  <v-layout column>
    <div class="text-center">
      <div class="mt-3 title font-weight-bold">
        ワインについて教えてください
      </div>
      <div class="mt-3 mb-3 caption grey--text">
        スライダーを選択してデータを入力してください。<br>
        データをもとにAIが診断します。
      </div>
    </div>
  </v-layout>
</template>

<script lang="ts">
import {Vue, Getter, Mutation, Component} from 'nuxt-property-decorator'

@Component({
  components: {
    FormCard: () => import('~/components/Form/FormCard.vue')
  }})
export default class Index extends Vue {
}
</script>

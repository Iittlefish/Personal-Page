<template>
  <v-container>
    <v-row class="text-center">
      <v-spacer></v-spacer>
      <v-col cols="12" v-for="(guessing,i) in guessing"
        :key="i"
        :question="guessing.question"
        :ans="guessing.ans"
      >
          <v-card height="120"
            elevation="2"
            outlined
            shaped
             align-center
            >
            <v-card-title>
              {{guessing.question  }}
            </v-card-title>
            <v-card-text>
              {{guessing.ans}}
            </v-card-text>
          </v-card>
      </v-col>
    </v-row>
    <router-link to='about'>
      <v-btn elevation="2">about</v-btn>
    </router-link>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'HelloWorld',

  data: () => ({
    guessing: [
      {
        question: '五月花和百合花哪一個沒有生小孩？',
        ans: '五月花。因為五月花衛生紙(未生子)。',
      },
      {
        question: '如果跟吳宗憲打籃球，應該找誰來防守他？',
        ans: '慈母，因為慈母守宗憲。',
      },
      {
        question: '為啥美人魚最專情？',
        ans: '因為他不會劈腿。',
      },
      {
        question: '有兩個人掉到陷阱裡了，死掉的人叫死人，活人叫什麼？',
        ans: '救命',
      },
    ],
  }),
});
</script>

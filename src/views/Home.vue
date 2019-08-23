<template>
  <div class="bkg">

    <v-layout column align-center justify-center class="white--text">

      <img src="../assets/coclogowithname.png" alt="Vuetify.js" height="auto" class="hidden-sm-and-down" width="80%">
      <img src="../assets/coc_logo.png" alt="Vuetify.js" height="200" class="hidden-md-and-up">
      <h1 class="white--text mb-2 display-1 text-xs-center">PRESENTS</h1>
      <div class="mb-3 text-xs-center ws"><v-icon dark x-large>mdi-code-not-equal-variant</v-icon>&nbsp;Competitive Coding Workshop&nbsp;<v-icon dark x-large>mdi-code-not-equal-variant</v-icon></div>

    </v-layout>

    <v-divider dark></v-divider>
    
    <br>
    <h1 class="text-xs-left ws white--text ml-4"><u>Problems:</u></h1>

    <v-layout align-center justify-center class="white--text">
      <v-flex md6>
        <v-simple-table class="table mt-4 mb-4">
          <thead>
            <tr>
              <th class="text-center white--text">Arrays-Strings</th>
              <th class="text-left white--text">Difficulty</th>
              <th class="text-left white--text">Try Out</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in items1" :key="item.problem">
              <td>{{ item.problem }}</td>
              <td :class="item.color">{{ item.difficulty }}</td>
              <td><a :href='item.to' target='_blank'><v-btn ><v-icon>mdi-border-color</v-icon></v-btn></a></td>
            </tr>
          </tbody>
        </v-simple-table>
      </v-flex>

    </v-layout>

    <v-layout align-center justify-center class="white--text">
      <v-flex md6>
        <v-simple-table class="table mt-4 mb-4">
          <thead>
            <tr>
              <th class="text-center white--text">Sorting-Greedy</th>
              <th class="text-left white--text">Difficulty</th>
              <th class="text-left white--text">Try Out</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in items2" :key="item.problem">
              <td>{{ item.problem }}</td>
              <td :class="item.color">{{ item.difficulty }}</td>
              <td><a :href='item.to' target='_blank'><v-btn ><v-icon>mdi-border-color</v-icon></v-btn></a></td>
            </tr>
          </tbody>
        </v-simple-table>
      </v-flex>
    </v-layout>

    <v-layout align-center justify-center class="white--text">
      <v-flex md6>
        <v-simple-table class="table mt-4 mb-4">
          <thead>
            <tr>
              <th class="text-center white--text">Recursion</th>
              <th class="text-left white--text">Difficulty</th>
              <th class="text-left white--text">Try Out</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in items3" :key="item.problem">
              <td>{{ item.problem }}</td>
              <td :class="item.color">{{ item.difficulty }}</td>
              <td><a :href='item.to' target='_blank'><v-btn ><v-icon>mdi-border-color</v-icon></v-btn></a></td>
            </tr>
          </tbody>
        </v-simple-table>
      </v-flex>
    </v-layout>

    <v-layout align-center justify-center class="white--text">
      <v-flex md6>
        <v-simple-table class="table mt-4 mb-4">
          <thead>
            <tr>
              <th class="text-center white--text">DP-HashTable</th>
              <th class="text-left white--text">Difficulty</th>
              <th class="text-left white--text">Try Out</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in items4" :key="item.problem">
              <td>{{ item.problem }}</td>
              <td :class="item.color">{{ item.difficulty }}</td>
              <td><a :href='item.to' target='_blank'><v-btn ><v-icon>mdi-border-color</v-icon></v-btn></a></td>
            </tr>
          </tbody>
        </v-simple-table>
      </v-flex>
    </v-layout>

  </div>
</template>

<script>

export default {
  data () {
    return {
      items1: [
        {
          problem: 'Check if a given string is Palindrome',
          difficulty: 'SCHOOL',
          color: 'primary--text',
          to: 'https://practice.geeksforgeeks.org/problems/palindrome-string/0'
        },
        {
          problem: 'Reverse a given string',
          difficulty: 'SCHOOL',
          color: 'primary--text',
          to: 'https://practice.geeksforgeeks.org/problems/reverse-the-string/0'
        },
        {
          problem: 'Reverse words in a given string',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/reverse-words-in-a-given-string/0'
        },
        {
          problem: 'Param Matching (w/o stack)',
          difficulty: 'EASY',
          color: 'success--text',
          to: '#'
        },
        {
          problem: 'Pair with a given sum',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/key-pair/0'
        },
        {
          problem: 'Sort array containing 0, 1, 2',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s/0'
        },
        {
          problem: 'Next greater (using stack)',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/next-larger-element/0'
        },
        {
          problem: 'Water trap	',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/trapping-rain-water/0'
        },
        {
          problem: 'Circular tour',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/circular-tour/1'
        },
      ],
      items2: [
        {
          problem: 'Coin Denomination',
          difficulty: 'EASY',
          color: 'success--text',
          to: '#'
        },
        {
          problem: 'Are 2 Strings Anagram?',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/anagram/0'
        },
        {
          problem: 'Join Ropes',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/minimum-cost-of-ropes/0'
        },
      ],
      items3: [
        {
          problem: 'Binary Search',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/binary-search/1'
        },
        {
          problem: 'Fast Exponentiation',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/modular-exponentiation-for-large-numbers/0'
        },
        {
          problem: 'Square Root (Binary Search)',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/square-root/1'
        },
      ],
      items4: [
        {
          problem: 'Nth Fibonacci',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/nth-fibonacci-number/0'
        },
        {
          problem: 'Are 2 Strings Anagram? (DP)',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/anagram/0'
        },
        {
          problem: 'Ways to climb a stair',
          difficulty: 'EASY',
          color: 'success--text',
          to: 'https://practice.geeksforgeeks.org/problems/count-number-of-hops/0'
        },
        {
          problem: 'Longest Increasing Subsequence',
          difficulty: 'MEDIUM',
          color: 'warning--text',
          to: 'https://practice.geeksforgeeks.org/problems/longest-increasing-subsequence/0'
        },
        {
          problem: 'Word Break',
          difficulty: 'HARD',
          color: 'error--text',
          to: 'https://practice.geeksforgeeks.org/problems/word-break/0'
        },
      ]
    }
  }
};
</script>

<style scoped>
  .bkg {
    background-color: #333;
  }
  .ws {
    font-size: 4em;
  }
  tbody tr:nth-of-type(odd) {
   background-color: rgba(0, 0, 0, .05);
  }
  thead {
    background-color: #2f4e4f;
  }
  .table {
    font-size: 2em;
  }
  th {
    font-size: 0.5em;
  }
</style>

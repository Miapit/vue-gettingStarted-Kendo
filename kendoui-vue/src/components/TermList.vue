<template>
  <div class="term-list">
    <div class="term-box">
      <div class="term">
        <h1> GIF </h1>
        <p class="term-definition">
          a lossless format for image files that support both animated and static images.
        </p>
        <div class="term-pronunciation">
          <input type="radio" v-model="selected" name="vote" :value="0" />
          <kendo-button
            icon='volume-up'
            @click='playSound("http://bit.ly/2HHjJio")'
            > gif
          </kendo-button>
          <kendo-button
            icon='volume-down'
            @click='playSound("http://bit.ly/2plm002")'
            > gif
          </kendo-button>
        </div>
        <div class="term-voting">
          <kendo-button class='k-primary' @click='onVote'>
            VOTE
          </kendo-button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'term-list',
  data () {
    return {
      selected: 0,
      pronunciation1Votes: 0,
      pronunciation2Votes: 0
    }
  },
  methods: {
    playSound (sound) {
      // if(sound){
      //   let audio = new Audio(sound)
      //   audio.play(play)
      // }
    },
    onVote () {
      alert()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>

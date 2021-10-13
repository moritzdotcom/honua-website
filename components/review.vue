<template>
  <div :class="review.id % 2 == 0 ? 'align-self-end text-right' : 'align-self-start text-left'" style="max-width: 80%">
    <div class="review-section m-5 content-card">
      <h5>{{review.title}}</h5>
      <b-icon v-for="star in review.stars" :key="star" icon="star-fill" variant="warning"></b-icon>
      <b-icon v-for="star in (5 - review.stars)" :key="star" icon="star"></b-icon>
      <p>
        {{review.content.split(' ').slice(0, 30).join(' ')}}
        <b-collapse :id="`collapse-${review.id}`" class="">
          {{review.content.split(' ').slice(30).join(' ')}}
        </b-collapse>
      </p>
      <a v-if="review.content.split(' ').length > 30" v-b-toggle="`collapse-${review.id}`" variant="primary"><span class="when-open">Weniger anzeigen</span><span class="when-closed">Mehr anzeigen</span></a>
    </div>
  </div>
</template>

<script>
  import { BIcon, BIconStar, BIconStarFill } from 'bootstrap-vue'
  import 'bootstrap-vue/dist/bootstrap-vue-icons.min.css'

  export default {
    props: ['review'],
    components: {
      BIcon,
      BIconStar,
      BIconStarFill
    }
  }
</script>

<style>
  .collapsed > .when-open,
  .not-collapsed > .when-closed {
    display: none;
  }

  .collapse.show {
    display: inline;
  }
</style>

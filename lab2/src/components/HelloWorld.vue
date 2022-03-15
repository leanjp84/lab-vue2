<template>
<div>
<div class="container">
  <div class="card" v-for="card in cards" v-bind:key="card.id">
    <div>
       <h2>{{card.title}}</h2>
      <p>{{card.content}}</p>
  </div>
  </div>
 </div>
</div>  
</template>

<script>
export default {
  data () {
    return {
      cards:[],
    }
  },
methods: {
  async getCards () {
    const res = await fetch ("http://localhost:3000/cards");
    const finalRes = await res.json();
    this.cards = finalRes;
  console.log(finalRes)
  },
},
 async mounted() {
  await this.getCards();
  },
}
</script>

<style>
.containter {
  width: 70%;
  display: flex;
  flex-direction: column;
}
.card {
  border:1px solid grey;
  border-radius: 5px;
  margin:20px;
  box-shadow: 3px 5px 10px 3px rgba(0, 0, 0, 0.4);
}
</style>

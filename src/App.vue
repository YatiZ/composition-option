<!-- Composition API -->
<!-- <template>
  <main>
    <div>
    <h4>The Current count is...</h4>
    <h1>{{count}}</h1>
    <button @click="count--">-</button>
    <button @click="count++">+</button>
    </div>  
  </main>
</template>

<style scoped>
 main{
  background-color:pink;
  justify-content: center;
  width: 100vw;
  height: 100vh;
 }
 div{
  text-align: center;
  margin-top: 100px;
 }
</style>

<script setup>
  import {ref} from "vue";
  const count = ref(0);
</script>
 -->

 <!-- option API -->
 <template>
  <h4>The current count is....</h4>
  <h1>{{ count }}</h1>
  <button @click="subtractCount()">-</button>
  <button @click="addCount()">+</button>
</template>

<style scoped>

</style>

<script>
export default({
  data(){
      return{
          count: 0
      }
  },
  methods:{
      addCount(){
          this.count = this.count+1
      },
      subtractCount(){
          this.count = this.count-1
      }
  }
})
</script>

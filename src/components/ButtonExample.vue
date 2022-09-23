<script setup lang="ts">
    defineProps()
</script>

<template>    
    <div class="button-example">
    <h1 class="green">Button example</h1>
    <h3>
        You clicked {{ count }} times. <br />
        <button @click="incrementCount">Click me!</button>
    </h3>
        
    </div>
</template>

<script lang="ts">
export default {
        data() {
            return {
                count: 0
            }
        },
        methods: {
            incrementCount() {
                this.count += 1
            }
        }
    }
</script>


<style scoped>
    h1 {
      font-weight: 500;
      font-size: 2.6rem;
      top: -10px;
    }
    
    h3 {
      font-size: 1.2rem;
    }
    
    .button-example h1 {
      text-align: center;
    }
    .button-example h3 {
      text-align: center;
    }
</style>
    
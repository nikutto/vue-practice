<script setup lang="ts">
    defineProps()
</script>

<template>    
    <div class="list-example">
    <h1 class="green">List example</h1>
    <h3>
        <table>
            <thead>
                <tr>
                    <th>name</th>
                    <th>age</th>
                    <th>timestamp</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="person in persons">
                    <td>{{person.name}}</td>
                    <td>{{person.age}}</td>
                    <td>{{person.timestamp}}</td>
                </tr>
            </tbody>
        </table>
    </h3>
    </div>
</template>

<script lang="ts">
export default {
        data() {
            return {
                persons: [
                    {name: "Bob", age: 14, timestamp: "2022/Sep/23"},
                    {name: "Alice", age: 22, timestamp: "2022/Sep/22"}
                ]
            }
        },
    }
</script>


<style scoped>
    table {
        margin-left: auto;
        margin-right: auto
    }
    table th{
        text-align: center;
        padding-left: 10px;
        padding-right: 10px;
    }

    h1 {
      font-weight: 500;
      font-size: 2.6rem;
      top: -10px;
    }
    
    h3 {
      font-size: 1.2rem;
    }
    
    .list-example h1 {
      text-align: center;
    }
    .list-example h3 {
      text-align: center;
    }

</style>
    
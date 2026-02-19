<template>
  <div>
    <h2>User Table</h2>
    <table border="1">
      <thead>
        <tr>
          <th>ID</th>
          <th>Name</th>
          <th>Email</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="user in users" :key="user.id">
          <td>{{ user.id }}</td>
          <td>
            <input v-model="user.name" />
          </td>
          <td>
            <input v-model="user.email" />
          </td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const users = ref([
  { id: 1, name: 'Eddy', email: 'eddy@example.com' },
  { id: 2, name: 'Alice', email: 'alice@example.com' },
  { id: 3, name: 'Bob', email: 'bob@example.com' },
  { id: 4, name: 'Charlie', email: 'charlie@example.com' },
  { id: 5, name: 'David', email: 'david@example.com' },
  { id: 6, name: 'Eve', email: 'eve@example.com' },
  { id: 7, name: 'Frank', email: 'frank@example.com' },
  { id: 8, name: 'Grace', email: 'grace@example.com' },
  { id: 9, name: 'Heidi', email: 'heidi@example.com' },
  { id: 10, name: 'Ivan', email: 'ivan@example.com' },
  { id: 11, name: 'Judy', email: 'judy@example.com' },
  { id: 12, name: 'Karl', email: 'karl@example.com' },
  { id: 13, name: 'Leo', email: 'leo@example.com' },
  { id: 14, name: 'Mallory', email: 'mallory@example.com' },
  { id: 15, name: 'Nina', email: 'nina@example.com' },
  { id: 16, name: 'Oscar', email: 'oscar@example.com' },
  { id: 17, name: 'Peggy', email: 'peggy@example.com' },
  { id: 18, name: 'Quentin', email: 'quentin@example.com' },
  { id: 19, name: 'Ruth', email: 'ruth@example.com' },
  { id: 20, name: 'Sybil', email: 'sybil@example.com' },
  
])
</script>
<style>
table {
  width: 100%;
  border-collapse: collapse;
}
th, td {
  padding: 8px;
  text-align: left;
}
input {
  width: 100%;
  box-sizing: border-box;
}
</style>
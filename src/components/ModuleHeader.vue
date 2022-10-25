<template>
  <div>
      <table>
          <tr>
              <th>{{text}}</th>
          </tr>
      </table>
  </div>
</template>

<script>
export default {
    props: ['text']
}
</script>

<style scoped>
table {
    border: 1px solid #000;
    border-collapse: collapse;
    width: 100%;
    margin-top: 10px;
    font-family: Arial, Helvetica, sans-serif;
}


</style>template
<template>
  <div>
    <h2>
      Hours
    </h2>
    <table class="d-flex justify-content-center mt-3">
      <tr>
        <th>Sunday</th>
        <td>Closed</td>
      </tr>
      <tr>
        <th>Monday</th>
        <td>Closed</td>
      </tr>
      <tr>
        <th>Tuesday</th>
        <td>11am - 6pm</td>
      </tr>
      <tr>
        <th>Wednesday</th>
        <td>8am - 1pm</td>
      </tr>
      <tr>
        <th>Thursday</th>
        <td>11am - 6pm</td>
      </tr>
      <tr>
        <th>Friday</th>
        <td>8am - 3pm</td>
      </tr>
      <tr>
        <th>Saturday</th>
        <td>Closed</td>
      </tr>
    </table>
  </div>
</template>


<script>
export default {
  setup() {
    return {}
  }
}
</script>


<style lang="scss" scoped>
table {
  border-spacing: 20px;
}

th,
td {
  padding-left: 20px;
  padding-right: 20px;
}

th {
  text-align: left;
}

td {
  text-align: right;
}
</style>
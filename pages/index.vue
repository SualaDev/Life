<template>
  <div class="container">
    <SaturnTable :data="tableData" />
  </div>
</template>

<script>
export default {
  data () {
    return {
      tableData: {
        title: 'Human Beings',
        headers: [
          { key: 'name', label: 'Name' },
          { key: 'address', label: 'Address' },
          { key: 'dob', label: 'Date of Birth', type: 'date/time' },
          { key: 'age', label: 'Age' },
          { key: 'balance', label: 'Account Balance', type: 'currency' },
          { key: 'isMarried', label: 'Marital Status' }
        ],
        labels: [
          {
            name: 'Favour Felix',
            address: '11b Oga Willi Road, Ebute Metta, Lagos',
            dob: 'Sat Jun 19 2021 17:31:23 GMT+0100 (West Africa Standard Time)',
            age: '10',
            balance: '500000',
            isMarried: true
          },
          {
            name: 'Emmanuel Felix',
            address: '11b Oga Willi Road, Ebute Metta, Lagos',
            dob: 'Sat Jun 19 2021 17:31:23 GMT+0100 (West Africa Standard Time)',
            age: '10',
            balance: '5000000',
            isMarried: true
          },
          {
            name: 'Constance Felix',
            address: '11b Oga Willi Road, Ebute Metta, Lagos',
            dob: 'Sat Jun 19 2021 17:31:23 GMT+0100 (West Africa Standard Time)',
            age: '10',
            balance: '500000',
            isMarried: true
          }
        ],
        styles: {
          fullWidth: true,
          actionText: 'See Person'
        }
      }
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  padding: 24px;
}
</style>

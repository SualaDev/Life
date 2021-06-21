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
          { key: '_id', label: 'ID', type: 'number', isFilterable: true },
          { key: 'name', label: 'Name', type: 'string', isFilterable: true },
          { key: 'address', label: 'Address', type: 'string', isFilterable: false },
          { key: 'dob', label: 'Date of Birth', type: 'date/time', isFilterable: true },
          { key: 'age', label: 'Age', type: 'number', isFilterable: true },
          { key: 'balance', label: 'Account Balance', type: 'currency', isFilterable: true },
          { key: 'isMarried', label: 'Marital Status', type: 'string', isFilterable: false }
        ],
        labels: [
          {
            _id: 1,
            name: 'Favour Felix',
            address: '44 nice Road, Ebute Metta, Lagos',
            dob: 'Jun 9 2021 15:33:13 GMT+0100 (West Africa Standard Time)',
            age: '23',
            balance: '30000',
            isMarried: true
          },
          {
            _id: 4,
            name: 'Emmanuel Felix',
            address: '11b Oga Willi Road, Lagos Island, Lagos',
            dob: 'May 8 2021 17:31:23 GMT+0100 (West Africa Standard Time)',
            age: '29',
            balance: '5000000',
            isMarried: true
          },
          {
            _id: 3,
            name: 'Constance Felix',
            address: '11b Oga Willi Road, Ebute Metta, Lagos',
            dob: 'July 18 2021 10:55:25 GMT+0100 (West Africa Standard Time)',
            age: '25',
            balance: '500000',
            isMarried: true
          }
        ],
        bulkActions: [
          { event: 'delete-people', name: 'Delete People' },
          { event: 'print-people', name: 'List People in CSV file' },
          { event: 'clean-people', name: 'Clean People' }
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

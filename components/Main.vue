<template>
  <el-main>
    <el-table :data="tableData">
      <el-table-column prop="date" label="Date" width="140"> </el-table-column>
      <el-table-column prop="name" label="Name" width="120"> </el-table-column>
      <el-table-column prop="address" label="Address"> </el-table-column>
    </el-table>
  </el-main>
</template>

<script>
export default {
  name: 'MainItem',
  data() {
    const item = {
      date: new Date().toLocaleDateString('en-US'),
      name: 'Nam',
      address: '03 Le Dinh Ly',
    }
    return {
      tableData: Array(20).fill(item),
    }
  },
}
</script>

<style></style>

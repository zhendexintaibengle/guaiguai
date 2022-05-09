<template>
  <div>
    <div class="new"><span @click="newT">新建</span></div>
    <div>
      <el-table :data="tableData" border style="width: 100%">
        <el-table-column prop="date" label="日期" width="180">
        </el-table-column>
        <el-table-column prop="name" label="姓名" width="180">
        </el-table-column>
        <el-table-column prop="address" label="地址"> </el-table-column>
      </el-table>
    </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        tableData: [{
          date: '2016-05-02',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1518 弄'
        }, {
          date: '2016-05-04',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1517 弄'
        }, {
          date: '2016-05-01',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1519 弄'
        }, {
          date: '2016-05-03',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1516 弄'
        },{
          date: '2016-06-03',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1520 弄'
        },{
          date: '2016-06-02',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1521 弄'
        },{
          date: '2016-06-01',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1516 弄'
        },
        {
          date: '2016-05-21',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1522 弄'
        }]
      }
    },
    methods: {
      newT() {
        
      }
    },
  }
</script>
<template>
  <div
    class="home"
    style="
       {
        height: 100vh;
        background: #0aa;
      }
    "
  >
    <el-container>
      <el-header>
        <div class="header">
          <div class="header-left">风险自查</div>
          <div class="header-right">
            <div class="name">姓名</div>
            <div class="touxiang">
              <img
                src="https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fb-ssl.duitang.com%2Fuploads%2Fitem%2F201901%2F11%2F20190111010348_tuyoj.jpg&refer=http%3A%2F%2Fb-ssl.duitang.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1654243437&t=211090bdeae61faf6b149e4d114bbacd"
                alt="头像"
              />
            </div>
          </div>
        </div>
      </el-header>
      <el-container class="container">
        <el-aside class="aside" width="200px">
          <el-col :span="12">
            <el-menu
              default-active="2"
              class="el-menu-vertical-demo"
              background-color="#545c64"
              text-color="#fff"
              active-text-color="#ffd04b"
            >
              <el-menu-item index="1" >
                <span slot="title">风险列表</span>
              </el-menu-item>
              <el-menu-item index="2">
                <span slot="title">BU首页</span>
              </el-menu-item>
            </el-menu>
          </el-col>
        </el-aside>
        <el-main>
          <table/>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import Table from '@/components/Table.vue';

export default {
  name: "",
  Table,
  components: {
    
  }
    
};
</script>

<style scoped>
.home {
  height: 100vh;
  background: #0aa;
}
.header {
  height: 100%;
  display: flex;
  align-items: center;
}
.header-right {
  display: flex;
  justify-content: flex-end;
  flex-grow: 1;
  align-items: center;
}
.name {
  padding-right: 8px;
}
.touxiang img {
  width: 40px;
  border-radius: 50%;
}
.el-col-12{
  width: 100%;
}
.container{
  height: calc(100vh - 60px);
  }
.aside{
  height: 100%;
  background: rgb(84, 92, 100);
  }
</style>


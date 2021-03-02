<template>
  <div>
    <h3>user</h3>
    <el-button>点击</el-button>
    <el-dialog title="test"
               :visible.sync="testData">
      <el-form :model="addForm"
               :rules="addFormRules"
               ref="addFormRef"
               label-width="70px">
        <el-form-item label="用户名"
                      prop="username">
          <el-input></el-input>
        </el-form-item>
        <el-form-item label="密码"
                      prop="password">
          <el-input></el-input>
        </el-form-item>
        <el-form-item label="邮箱"
                      prop="email">
          <el-input></el-input>
        </el-form-item>
        <el-form-item label="手机"
                      prop="mobile">
          <el-input></el-input>
        </el-form-item>
      </el-form>
    </el-dialog>
  </div>
</template>

<script>
export default {
  data () {
    return {
      testData: true
    }
  }
}
</script>

<style>
</style>

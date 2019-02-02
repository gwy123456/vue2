<template>
  <div class="box">
    <!-- login.vue -->
    <div class="content">
        <!-- 表单组件 -->
      <el-form
        :model="ruleForm2"
        status-icon
        ref="ruleForm2"
        label-width="100px"
        class="demo-ruleForm"
      >
        <el-form-item label="用户名">
          <el-input type="text" v-model="ruleForm2.pass" autocomplete="off"></el-input>
        </el-form-item>
        <el-form-item label="密码" prop="checkPass">
          <el-input type="password" v-model="ruleForm2.checkPass" autocomplete="off"></el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" @click="submitForm('ruleForm2')">提交</el-button>
          <el-button @click="resetForm('ruleForm2')">重置</el-button>
        </el-form-item>
      </el-form>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            loginObj: {
                
            }
        }
    }
};
</script>

<style>
.box {
  width: 100%;
  height: 100%;
  background-color: #2c3742;
  position: relative;
}
.box .content {
  width: 500px;
  padding: 40px;
  background-color: #fff;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border-radius: 5px;
}
</style>

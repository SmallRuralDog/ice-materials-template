<template>
  <div class="user-layout container">
    <div class="header">
      <a href="#" class="meta">
        <img class="logo" src="https://img.alicdn.com/tfs/TB13UQpnYGYBuNjy0FoXXciBFXa-242-134.png" alt="logo" />
        <span class="title">飞冰</span>
      </a>
      <p class="desc">飞冰让前端开发简单而友好</p>
    </div>
    <div class="user-login">
      <div class="formContainer">
        <h4 class="formTitle">登 录</h4>
        <el-form>
          <el-form-item>
            <el-input placeholder="管理员账号" prefix-icon="el-icon-search" />
          </el-form-item>
          <el-form-item>
            <el-input placeholder="密码" prefix-icon="el-icon-search" />
          </el-form-item>
          <el-form-item>
            <el-checkbox v-model="value.checkbox">记住账号</el-checkbox>
          </el-form-item>
          <el-form-item>
            <el-button class="submitBtn" type="primary">登陆</el-button>
          </el-form-item>
        </el-form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  name: 'ogin',

  data() {
    return {
      value: {
        account: '',
        password: '',
        checkbox: false,
      },
    };
  },
  
  created() {},

  methods: {},
};
</script>
<style lang="scss" scoped>
.container {
  position: relative;
  width: 100%;
  height: 90vh;
  padding-top: 10vh;
  background: url(https://img.alicdn.com/tfs/TB1kOoAqv1TBuNjy0FjXXajyXXa-600-600.png)
    0% 0% / contain rgb(240, 242, 245);
}
.user-layout {
  .header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 40px;
  }
  .meta {
    display: flex;
    align-items: center;
    text-decoration: none;
  }
  .title {
    text-align: center;
    font-size: 33px;
    color: rgba(0, 0, 0, 0.85);
    font-family: 'Myriad Pro', 'Helvetica Neue', Arial, Helvetica, sans-serif;
    font-weight: 600;
  }
  .desc {
    margin: 10px 0;
    font-size: 14px;
    color: rgba(0, 0, 0, 0.45);
  }
  .logo {
    margin-right: 10px;
    width: 48px;
  }
  .formContainer {
    display: flex;
    justify-content: center;
    flex-direction: column;
    max-width: 368px;
    margin: 0 auto;
  }
  .formItem {
    position: relative;
    margin-bottom: 25px;
    flex-direction: column;
  }
  .formItemCol {
    position: relative;
    margin-bottom: 5px;
  }
  .formTitle {
    text-align: center;
    margin: 0 0 20px;
    color: rgba(0, 0, 0, 0.85);
    font-weight: bold;
  }
  .inputIcon {
    position: absolute;
    left: 12px;
    top: 50%;
    transform: translateY(-50%);
    color: #999;
  }
  .submitBtn {
    font-size: 16px;
    background: #3080fe;
    border-radius: 4px;
    width: 100%;
  }
  .checkbox {
    margin-left: 5px;
  }
  .tips {
    justify-content: center;
  }
  .link {
    color: #999;
    text-decoration: none;
    font-size: 13px;
  }
  .line {
    color: #dcd6d6;
    margin: 0 8px;
  }

  .next-input.next-input-single {
    width: 368px;
    height: 38px;
    line-height: 38px;
    input {
      padding-left: 32px;
      font-size: 13px;
    }
  }
  .next-checkbox-label {
    color: #999;
    font-size: 13px;
  }
}
</style>



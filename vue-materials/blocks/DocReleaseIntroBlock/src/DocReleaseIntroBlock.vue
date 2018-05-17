<template>
  <div class="wrapperContainer">
    <div class="bgImage2" />
    <div class="wrapper">
      <div class="bgImage">
        <div class="bgImageMask" />
      </div>
      <div class="wrapperBody">
        <div class="softwareIntro">
          <div class="title">
            Iceworks
            <span class="subtitle"></span>
          </div>
          <div class="slogan">让前端工程变的轻松便捷</div>
          <div style="margin-left:-45px;padding-top:45px;textAlign: center">
            <el-dropdown>
              <el-button round plain>
                立即下载
                <span>For MacOS</span>
                <i class="el-icon-arrow-down el-icon--right"></i>
              </el-button>
              <el-dropdown-menu slot="dropdown">
                <el-dropdown-item>For MacOS 版本</el-dropdown-item>
                <el-dropdown-item>For Windows 版本(64位)</el-dropdown-item>
              </el-dropdown-menu>
            </el-dropdown>
          </div>
          <div class="softwareDetail">
            <div class="version">
              <span style="display: block;font-size:12px;">1.6.2</span>
              <span style="display: block; font-size: 12px; ">当前版本</span>
            </div>
            <div class="separator" />
            <div class="history">
              <span style="display: block;font-size:12px;">2018-04-23</span>
              <span style="display: block; font-size: 12px">
                发布日期
              </span>
            </div>
          </div>
          <div style="padding-top: 20px;width: 200px; text-align: center;">
            <div style="font-size: 12px; color: #fff">运行环境：macOS 10.9 及以上</div>
          </div>
          <div style="padding-top: 20px;text-align: center; width: 200px; ">
            <a style="color: #fff">立即开始</a>
          </div>
        </div>
        <div class="software" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  name: 'DocReleaseIntroBlock',
  data() {
    return {};
  },

  created() {},

  methods: {},
};
</script>

<style lang="scss">
.wrapperContainer {
  height: 750px;
  position: relative;
  overflow: hidden;
}
.bgImage2 {
  width: 1400px;
  height: 782px;
  border-radius: 391px;
  background: linear-gradient(
    135deg,
    rgb(94, 136, 255) 0%,
    rgb(111, 48, 254) 100%
  );
  transform: rotate(-45deg);
  box-shadow: rgba(0, 0, 0, 0.06) 2px 2px 60px;
  position: absolute;
  left: 35%;
  bottom: 550px;
  z-index: 1;
}
.wrapper {
  height: 750px;
  background-color: #f6f6f6;
  position: relative;
  width: 100%;
}
.wrapperBody {
  max-width: 1190px;
  height: 750px;
  position: relative;
  margin: 0 auto;
  z-index: 2;
}
.softwareIntro {
  position: absolute;
  left: 5%;
  padding-top: 230px;
  z-index: 3;
}
.title {
  font-size: 46px;
  color: #fff;
  font-weight: 500;
  line-height: 66px;
  text-shadow: 0 0 3px rgba(0, 0, 0, 0.3);
  margin-bottom: 16px;
}
.slogan {
  font-size: 24px;
  color: #fff;
  line-height: 34px;
  text-shadow: 0 0 3px rgba(0, 0, 0, 0.3);
}
.softwareDetail {
  padding-top: 24px;
  display: flex;
  flex-direction: row;
  color: #fff;
  font-size: 14px;
  font-weight: 100;
  width: 200px;
  justify-content: space-between;
  align-items: center;
}
.software {
  background-image: url(//img.alicdn.com/tfs/TB1uPagpQyWBuNjy0FpXXassXXa-1446-1148.png);
  width: 723px;
  height: 574px;
  background-size: 723px 574px;
  position: absolute;
  top: 100px;
  left: 38%;
}
.separator {
  width: 1px;
  height: 20px;
  background-color: #fff;
}
.version {
  width: 80px;
  line-height: 20px;
  text-align: center;
}
.history {
  width: 80px;
  line-height: 20px;
  text-align: center;
}
.bgImage {
  position: absolute;
  width: 100%;
  height: 750px;
  background-size: cover;
  background-image: url('//img.alicdn.com/tfs/TB1eoehpKOSBuNjy0FdXXbDnVXa-3798-1500.jpg');
}
.subtitle {
  font-size: 16px;
  font-weight: normal;
}
.bgImageMask {
  width: 100%;
  height: 750px;
  background: linear-gradient(
      135deg,
      rgba(94, 136, 255, 0.85) 0%,
      rgba(111, 48, 254, 0.85) 100%
    )
    /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */;
}
</style>


<template>
  <div class="leftNavbar side-menu sidebar-inverse">
    <a href="login.html" class="mainLogo">
      <div class="logo2">
      </div>
      <h4>云文件管理系统</h4>
    </a>
    <ul class="leftMenu">
      <li class="leftNav">
        <a href=""><span class="home navLeftIcon"><span class="homeIcon"></span></span>首页 </a>
      </li>
      <li class="leftNav">
        <a href="#"><span class="company navLeftIcon"><span class="companyIcon"></span></span>公司管理<span
          class="navLeftIcon2"></span></a>
        <ul class="leftNavSubWrap">
          <li class="leftNav leftNavSub"><a href="companyManage.html">公司管理</a></li>
          <li class="leftNav leftNavSub"><a href="modifyCompany.html">新增/修改</a></li>
        </ul>
      </li>
      <li class="leftNav">
        <a href="#"><span class="contract navLeftIcon"><span class="contractIcon"></span></span>合同管理<span class="navLeftIcon2"></span></a>
        <ul class="leftNavSubWrap">
          <li class="leftNav leftNavSub"><a href="contractManage.html">合同管理</a></li>
          <li class="leftNav leftNavSub"><a href="addContract.html">新增 / 修改</a></li>
          <li class="leftNav leftNavSub"><a href="invitationDetail.html">邀请详情</a></li>
        </ul>
      </li>
      <li class="leftNav">
        <a href="#"><span class="batch navLeftIcon"><span class="batchIcon"></span></span>批次管理<span
          class="navLeftIcon2"></span></a>
        <ul class="leftNavSubWrap">
          <li class="leftNav leftNavSub"><a href="batchManage.html">批次管理</a></li>
          <li class="leftNav leftNavSub"><a href="addBatch.html">新建批次</a></li>
        </ul>
      </li>
      <li class="leftNav">
        <a href="#"><span class="batch navLeftIcon"><span class="userIcon"></span></span>用户管理<span
          class="navLeftIcon2"></span></a>
        <ul class="leftNavSubWrap">
          <li class="leftNav leftNavSub"><a href="userManage.html">用户管理</a></li>
        </ul>
      </li>
    </ul>
    <div class="exit">
      <span><span class="exitIcon"></span><a href="">退出</a></span>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'leftNav',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" >
  @import "../../static/css/same";
  .logo2 {
    width: 36px;
    height: 24px;
    margin:35px;
    background: url(../assets/logo2.png) 50% 50% no-repeat;
  }

  .mainLogo {
    position: fixed;
    display: inline-block;
    width: 248px;
    height: 100px;
    background-color: #535f6b;
    z-index: 999;
    left:0;
    ul {
      width: 248px;
      height: 24px;
      line-height: 24px;
      margin-left: 40px;
      li {
        display: inline-block;
        margin-top: 35px;
      }
    }
    h4 {
      position: absolute;
      right: 50px;
      top: 0;
      color: white;
      line-height: 98px;
      font-size: 16px;
      margin-top: 0;
      margin-bottom: 0;
    }
  }

  .leftNavbar {
    width: 248px;
    height: 100%;
    position: fixed;
    top: 0;
    background: $backgroundDark;
    z-index: 10000;
    ul {
      padding: 0;
      text-decoration: none;
    }
  }
  .leftMenu {
    margin-top: 98px;
  }

  .leftNav {
    display: inline-block;
    position: relative;
    width: 100%;
    line-height: 60px;
    text-align: center;
    background: #252a2e;
    border-bottom: 1px solid $backgroundDark;
  a {
    color: #fff;
    display: block;
    width: 246px;
    height: 60px;
    text-decoration: none;
    transition: all 0.4s;
            -moz-transition: all 0.4s;
            -webkit-transition: all 0.4s;
            -o-transition: all 0.4s;
  &:hover {
     display: inline-block;
     width: 100%;
     height: 60px;
     background-color: #1451a5;
     color: #fff;
     text-decoration: none;
   }
  span {
    span {
      display: block;
      width: 20px;
      height: 20px;
    }
  }
    .homeIcon {
      background: url(../assets/EBC.png) no-repeat -181px -114px
    }
    .companyIcon {
      background: url(../assets/EBC.png) no-repeat -95px -114px
    }
    .contractIcon {
      background: url(../assets/EBC.png) no-repeat -124px -114px
    }
    .batchIcon {
      background: url(../assets/EBC.png) no-repeat -152px -114px
    }
    .userIcon {
      background: url(../assets/EBC.png) no-repeat -256px -114px
    }
  }
    .leftNavSubWrap {
      display: none;
    }
    .leftNavSub {
      border: none;
      background-color: $backgroundDark;
  }
    .navLeftIcon {
      position: absolute;
      left: 65px;
      top: 20px;
    }
    .navLeftIcon2 {
      background: url(../assets/EBC.png) no-repeat -234.3px -114px;
      position: absolute;
      top: 25px;
      right: 24px;
      width: 8px;
      height: 16px;
    }
  }

  .exit {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 248px;
    height: 58px;
    color: #c5c6ca;
    background: #535f6b;
    line-height: 58px;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    a {
      color: #fff;
      text-decoration: none;
      width: 20px;
      height: 20px;
      text-align: center;
    }
    .exitIcon {
      background: url(../assets/EBC.png) no-repeat -69px -114px;
      display: block;
      width: 20px;
      height: 20px;
      float: left;
      position: relative;
      top: 20px;
    }
  }
</style>

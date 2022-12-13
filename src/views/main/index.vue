<template>
  <!-- 主体容器 -->
  <main class="container">
    <!-- 头部区域 -->
    <div class="header">
      <!-- 头像 -->
      <div class="avatar">
        <img
          src="https://prd.storage.lit.link/images/creator/d6431197-40bf-423d-affc-08cac3713761/696bada4-8922-412b-bbcb-862fb18e8e99.jpeg"
          alt="avatar"
        />
      </div>
      <!-- 昵称 -->
      <div class="nickname">周_amane</div>
      <!-- 简介 -->
      <div class="intro">現役日本JK</div>
      <!-- 描述 -->
      <div class="description">
        現役日本JK<br />
        恋をすると人間になるらしい＿＿＿＿
      </div>
    </div>
    <!-- 社交账号 -->
    <div class="sns">
      <a class="sns-item" v-for="item in 5" :key="item">
        <div class="sns-item-container">
          <!-- 社交账号图片  -->
          <div class="sns-item-icon">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 210 210"
              class="injected-svg"
              data-src="https://prd.storage.lit.link/images/assets/icons/btn/icon-twitter.svg"
              xmlns:xlink="http://www.w3.org/1999/xlink"
            >
              <path
                d="M80.691,158.925c49.948,0,77.269-41.38,77.269-77.269,0-1.176,0-2.352-.073-3.518a55.1,55.1,0,0,0,13.545-14.059,53.936,53.936,0,0,1-15.593,4.273,27.228,27.228,0,0,0,11.939-15.025,54.249,54.249,0,0,1-17.241,6.594A27.174,27.174,0,0,0,103.549,78.5a26.686,26.686,0,0,0,.7,6.195A77.108,77.108,0,0,1,48.267,56.34a27.184,27.184,0,0,0,8.4,36.257,27,27,0,0,1-12.285-3.423v.346a27.174,27.174,0,0,0,21.787,26.628,27.276,27.276,0,0,1-7.161.956,26.253,26.253,0,0,1-5.1-.494,27.184,27.184,0,0,0,25.368,18.9,54.883,54.883,0,0,1-40.2,11.246,76.845,76.845,0,0,0,41.632,12.2"
              ></path>
            </svg>
          </div>
          <!-- 内容 -->
          <div class="sns-item-main">
            <!-- 标题 -->
            <div class="sns-item-main-title">Twitter</div>
            <div class="sns-item-main-desc">日常呟く！！</div>
          </div>
        </div>
      </a>
    </div>
  </main>
</template>

<script setup lang="ts">
const a = 10;
</script>

<style lang="scss" scoped>
/* 容器 */
.container {
  width: 480px;
  max-width: 480px;
  // height: 500px;
  // background-color: red;
}

/* 头部区域 */
.header {
  margin-top: 20px;
  // 头像
  .avatar {
    display: flex;
    justify-content: center;
    img {
      width: 120px;
      height: 120px;
      border-radius: 50%;
    }
  }

  // 昵称
  .nickname {
    font-size: 16px;
    color: rgb(142, 141, 141);
    font-weight: 700;
    text-align: center;
    margin-top: 14px;
  }

  // 简介
  .intro {
    font-size: 14px;
    color: rgb(142, 141, 141);
    font-weight: 700;
    text-align: center;
    margin-top: 6px;
  }

  // 描述
  .description {
    text-align: center;
    font-size: 12px;
    font-weight: 700;
    color: rgb(142, 141, 141);
    margin-top: 14px;
  }
}

// 社交账号
.sns {
  margin-top: 20px;
  .sns-item {
    display: block;
    width: 100%;
    height: 70px;
    color: rgb(142, 141, 141);
    background: rgb(255, 255, 255);
    padding: 7px;
    border-radius: 8px;
    margin-bottom: 14px;

    &:last-child {
      margin-bottom: 0px;
    }
  }

  .sns-item-container {
    display: flex;
    .sns-item-icon {
      width: 56px;
      height: 56px;
      margin-right: 12px;
      border-radius: 9px;
      box-shadow: rgb(0 0 0 / 16%) 0px 3px 6px;

      svg,
      img {
        width: 100%;
        height: 100%;
      }
      svg {
        fill: rgb(142, 141, 141);
      }
    }
  }

  .sns-item-main {
    display: flex;
    flex-direction: column;
    padding: 3px 0px 0px;
    color: rgb(142, 141, 141);
    font-weight: 700;

    .sns-item-main-title {
      font-size: 14px;
    }
    .sns-item-main-desc {
      font-size: 12px;
      margin: 3px 0px 0px;
    }
  }
}
</style>

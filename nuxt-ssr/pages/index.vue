<template>
  <div class="container">
    <div>
      <logo />
      <h1 class="title">[ CloudBase + Nuxt ] Fullstack APP</h1>
      <h2 class="subtitle">云开发 CloudBase + Nuxt SSR 全栈应用，包含前端网站 + 云开发函数</h2>
      <div class="links">
        <a href="https://cloudbase.net/" target="_blank" class="button--green">云开发 CloudBase 文档</a>
        <a href="https://nuxtjs.org/" target="_blank" class="button--green">Nuxt 文档</a>
        <a href="https://github.com/nuxt/nuxt.js" target="_blank" class="button--grey">GitHub</a>
      </div>

      <h2>本示例 Github 源码地址：</h2>
      <a
        href="https://github.com/TencentCloudBase/cloudbase-templates/tree/master/nuxt-ssr"
      >https://github.com/TencentCloudBase/cloudbase-templates/tree/master/nuxt-ssr</a>
      <h2>
        开发部署工具: CloudBase Framework
        <a
          href="https://github.com/TencentCloudBase/cloudbase-framework"
        >
          <img
            alt="CloudBase Framework"
            src="https://img.shields.io/github/stars/TencentCloudBase/cloudbase-framework?style=social"
          />
        </a>
      </h2>
      <a
        href="https://github.com/TencentCloudBase/cloudbase-framework"
        title="CloudBase Framework: 云开发前后端一体化部署工具"
      >
        <img width="420" src="https://main.qcloudimg.com/raw/615038b16047fa677646011fae909102.png" />
      </a>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo,
  },

  data() {
    return {
      isLoginSuccss: null,
      envId: "",
      callFunctionResult: "",
    };
  }
};
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.links a {
  margin-bottom: 8px;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 40px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 400;
  font-size: 20px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

h2,
p {
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

h2 {
  padding: 20px;
}

a {
  color: #3b8070;
}
</style>

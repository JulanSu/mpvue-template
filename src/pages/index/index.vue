<template>
  <div>
    <p class="title" @click="toNext">
      我是第一个
      <span>调往下一个页面</span>
    </p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: "mpvue"
    };
  },

  methods: {
    toNext() {
      mpvue.navigateTo({
        url: "/pages/log/main"
      });
    }
  },

  created() {
    let app = getApp();
  }
};
</script>

<style scoped lang="scss">
.userinfo {
  display: flex;
  flex-direction: column;
  align-items: center;
}
p {
  width: 40px;
  height: 30px;
  span {
    color: #f00;
  }
}
</style>

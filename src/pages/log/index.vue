<template>
  <div @click="clickHandle">
    <p class="title" @click="toBack">
      我是第二个页面
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
    toBack() {
      mpvue.navigateBack();
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

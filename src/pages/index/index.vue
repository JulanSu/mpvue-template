<template>
  <div @click="clickHandle">
    <p class="title">
      我是第一个
      <span>我是第二个</span>
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
    tt() {
      console(11123);
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

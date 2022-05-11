<template>
  <div class="HelloWorld">
    <div class="areadatavueoutbox">
      <div>1.area-data-vue</div>
      <area-select
        v-model="selected"
        :data="$pcaa"
        :level="0"
        @change="GetChangeFun"
      ></area-select>
      // 省
      <area-select
        v-model="selected"
        :data="$pcaa"
        :level="1"
        @change="GetChangeFun"
      ></area-select>
      // 省市
      <area-select
        v-model="selected"
        :data="$pcaa"
        :level="2"
        @change="GetChangeFun"
      ></area-select>
      // 省市区：
      <area-select
        v-model="selected"
        :data="$pcaa"
        :level="3"
        @change="GetChangeFun"
      ></area-select>
      // 省市区街道：

      <area-cascader
        v-model="selected2"
        :data="$pcaa"
        :level="0"
        @change="GetChangeFun"
      ></area-cascader>
      // 省市
      <area-cascader
        v-model="selected2"
        :data="$pcaa"
        :level="1"
        @change="GetChangeFun"
      ></area-cascader>
      // 省市区：
      <area-cascader
        v-model="selected2"
        :data="$pcaa"
        :level="2"
        @change="GetChangeFun"
      ></area-cascader>
      // 省市区街道：
    </div>
  </div>
</template>
<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      selected: [],
      selected2: [],
    };
  },
  methods: {
    GetChangeFun(val) {
      console.log("GetChangeFun", val);
    },
  },
};
</script>
<style lang="scss" scoped>
.HelloWorld {
}
</style>

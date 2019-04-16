<template>
  <span class="so-breadcrumb_item" ref="link">
    <a :href="to" class="label-name">
      <slot></slot>
    </a>
    <i v-if="separatorClass" class="separator_icon" :class="separatorClass"></i>
    <span v-else class="separator">{{separator}}</span>
  </span>
</template>
<style scoped>
.so-breadcrumb_item {
  font-size: 14px;
  color: #303133;
}
.separator {
  color: #c0c4cc;
  margin: 0 9px;
  font-weight: 700;
}
.label-name {
  color: #303133;
  font-weight: 700;
}
.separator_icon {
  margin: 0 9px;
  color: #c0c4cc;
}
</style>
<script>
export default {
  name: "",
  //   props: {
  //     to: {},
  //     replace: Boolean
  //   },
  props: ["to"],
  data() {
    return {
      separator: "",
      separatorClass: ""
    };
  },
  inject: ["Sobreadcrumb"],
  /** 载入后 */
  mounted() {
    this.separator = this.Sobreadcrumb.separator;
    this.separatorClass = this.Sobreadcrumb.separatorClass;
  },
  methods: {}
};
</script>



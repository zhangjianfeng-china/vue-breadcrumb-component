<template>
  <div class="so-breadcrumb">
    <slot></slot>
  </div>
</template>
<style>
.so-breadcrumb_item:last-child .separator {
  display: none;
}
.so-breadcrumb_item:last-child .label-name {
  color: #606266;
}
.so-breadcrumb_item:last-child .separator_icon {
  display: none;
}
</style>
<script>
export default {
  name: "Sobreadcrumb",
  //   props: {
  //     separator: {
  //       type: "String",
  //       default: "/"
  //     }
  //   },
  props: ["separator", "separatorClass"],
  /** separatorClass 为分割线的样式 */

  data() {
    return {};
  },
  provide() {
    return {
      Sobreadcrumb: this
    };
  },
  methods: {}
};
</script>



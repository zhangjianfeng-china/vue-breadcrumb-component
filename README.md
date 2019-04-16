#在全局注册该组件：

```
import breadcrumb from './components/breadcrumb/src/breadcrumb.vue';
import breadcrumb_item from './components/breadcrumb/src/breadcrumb-item.vue';
Vue.component('v-breadcrumb', breadcrumb);
Vue.component('v-breadcrumb-item', breadcrumb_item);
```

#调用：
```
<v-breadcrumb separator="/" separatorClass="fa fa-angle-right">
   <v-breadcrumb-item to="/">首页</v-breadcrumb-item>
   <v-breadcrumb-item to="/product">产品中心</v-breadcrumb-item>
</v-breadcrumb>
```


```
<v-breadcrumb>
Attributes : 
参数	                              说明	                                               类型	      可选值	        默认值 
separator                       面包屑分割线样式                                         String     
separatorClass                  图标分隔符 class（不能更separator同时使用）                                           

<v-breadcrumb-item>
Attributes:
参数	                              说明	                                               类型	      可选值	        默认值 
to                                路由跳转 放置vue路由                                   String
```
效果



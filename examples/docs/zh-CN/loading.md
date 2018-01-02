## Loading

<script>
  export default {
    data() {
      return {
        openLoading1: false,
        openLoading2: true,
        openLoading3: true
      }
    },
    
    methods: {
      toggle1() {
        this.openLoading1 = true;
        setTimeout(() => {
          this.openLoading1 = false;
        }, 3000);
      }
    }
  }
</script>

### 全屏loading
:::demo
```html
<template>
<el-button type="primary" @click="toggle1" v-loading.fullscreen="openLoading1">全屏Loading</el-button>
</template>
```
:::


### elem loading
:::demo
```html
<template>
    <div style="width: 100%; height: 100px;" v-loading="openLoading3"></div>
</template>
```
:::
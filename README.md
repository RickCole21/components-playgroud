# 爱速搭自定义组件本地开发环境

## 开发指南

```
# 安装依赖
npm i

# 开启本地服务
npm start
```

在对应的文件夹下，新建组件文件，并编写代码，例如：

- 在 `src/components/vue/formitem` 目录下新建文件，导入到爱速搭后，会解析为 **vue 表单项** 组件。
- 在 `src/util` 目录下新建文件，导入到爱速搭后，会解析为 **其他类型** 的组件。

> 文件支持 js、jsx、tsx 后缀

开发完成后，运行 `npm run build` 生成自定义组件压缩包 `components.zip` ，然后进入爱速搭 应用管理-自定义组件，点击「导入组件」，选中压缩包导入，等待编译完成后即可使用。

## 注意事项

导入到爱速搭解析时，会自动根据文件名生成对应的组件 key，并在前加 `custom-` 前缀。

例如：一个名字为 `vue-text.js` 的组件文件，导入后，是通过 `custom-vue-text` 来使用的。

所以组件的文件名不可以重复

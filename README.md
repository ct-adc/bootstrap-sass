## 说明

该版本取bootstrap V3.3.7作为基础版本，对其进行针对项目的版本改造，并发布到内部cdn上供公司项目开发使用

## 修改方法

css的修改:

1. 修改assets/stylesheets/custom中的_bootstrap-variables和style文件。
_bootstrap-variables: bootstrap样式公用变量
style: 另外新增的自定义样式

2. 运行`npm run css-build` 和 `npm run css-min-build`，用于生成非压缩版和压缩版样式，
   生成的样式会被写入到assets/css中

3. 将assets/css中的文件上传到内部cdn: `ftpPath`/CtStatic/cdn/bootstrap/3.3.7/custom/1.0.0/css

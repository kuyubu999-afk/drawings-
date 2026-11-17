# 东方水墨 Studio（Android）

本仓库包含一个 Kotlin 原生 Android 水墨画创作原型。

## 功能
- 从设备选择图片
- 居中比例裁剪（原比例、1:1、4:3、3:4、16:9）
- 六种历史画家风格参考入口
- 本地灰度、边缘与纸色处理
- 中文题款和朱红印章框
- PNG 保存到相册
- 不上传用户图片

## 自动构建
向 `main` 分支推送后，GitHub Actions 会解码项目归档、构建 Debug APK，并将其作为 `InkWashStudio-debug-apk` artifact 上传。也可以在 Actions 页面手动运行工作流。

## 源码归档
`InkWashStudio_Android_MVP.zip.b64` 是项目 ZIP 的 Base64 文本归档，由工作流自动还原。下载后可用 Base64 解码并解压，或直接通过 GitHub Actions 获取构建产物。

## 当前原型限制
风格选项是参数化的传统图像处理效果，并非生成式 AI 或对历史画家笔法的精确复刻。裁剪目前为居中比例裁剪。

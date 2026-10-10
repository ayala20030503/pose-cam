# POSE CAM 原型（跨 iPhone / Android）

## 功能
- 实时摄像头预览
- 导入参考照片并叠加到取景框
- 模板透明度、大小调节；拖动模板改变位置
- 三分构图网格
- 前后摄像头切换
- 拍照并保存真实相机画面（不包含模板辅助层）

## 重要说明
浏览器摄像头通常要求安全上下文：HTTPS 或 localhost。不要只把 `index.html` 作为普通 HTTP 网页打开。
此原型不上传照片；模板和拍摄均在浏览器本地处理。不同手机/浏览器对保存下载文件的行为可能不同。

## 最快试用：GitHub Pages
1. 登录 GitHub，新建一个公开仓库，例如 `pose-cam`.
2. 将 `index.html` 上传到仓库根目录并提交。
3. 打开仓库 Settings → Pages。
4. 在 Build and deployment 选择 `Deploy from a branch`，分支选择 `main`，目录选 `/ (root)`，保存。
5. 等待发布完成，打开 GitHub Pages 提供的 `https://...github.io/pose-cam/` 地址。
6. 用 iPhone 的 Safari 或安卓 Chrome 打开并允许相机权限。

如果不想使用 GitHub，也可以把 `index.html` 部署到支持静态网页和 HTTPS 的托管服务。

## 后续建议
1. 真机测试不同设备的摄像头权限、切换前后摄像头、竖屏取景比例。
2. 增加模板库、构图参考线、拍摄前后对比。
3. 若希望像原生相机一样稳定、直接保存系统相册、后台行为更完整，再评估 Capacitor 等跨平台封装。

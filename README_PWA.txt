选调备考控制台 · PWA版
========================

这版已经加入：
- Web App Manifest
- Service Worker 离线缓存
- 安卓可安装提示
- iPhone“添加到主屏幕”适配
- 192/512/maskable/Apple Touch 图标
- 保留原 localStorage 数据、30天计划、计时、错题、复盘、模考等全部功能

重要：PWA 安装需要通过 HTTPS 打开。直接点本地 index.html 或用“HTML阅读器”只能预览，不能成为真正 PWA。

最推荐：把本文件夹完整上传到任意 HTTPS 静态网站空间，保持文件相对位置不变。然后手机用 Safari/Chrome 打开该 HTTPS 地址一次。

安卓 Chrome/Edge：
1. 用 HTTPS 地址打开。
2. 进入“设置/备份”页，若“安装 App”按钮可用则直接点。
3. 或浏览器菜单 → “安装应用/添加到主屏幕”。
4. 安装后可从桌面进入；首次缓存完成后可离线使用。

iPhone Safari：
1. 用 Safari 打开 HTTPS 地址。
2. 点“分享”。
3. 选择“添加到主屏幕”。
4. 从桌面图标启动。

数据说明：
- 学习记录仍只保存在当前手机的浏览器/PWA localStorage。
- 清浏览器站点数据、卸载并清除站点数据前，请先“导出JSON备份”。
- 手机和电脑不会自动同步，需要使用导出/导入JSON。

电脑本地测试：
在本文件夹中执行： python -m http.server 8000
电脑自己访问 http://localhost:8000/index.html 可测试 Service Worker/PWA。
但手机访问电脑的 http://192.168.x.x:8000 通常不属于安全上下文，只适合浏览测试，不建议用于正式安装 PWA。

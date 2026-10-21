# 健哥快乐空间 PWA

这是完整 PWA 文件包。包含：
- index.html：个人记录网页
- manifest.webmanifest：App 图标、名称、全屏/独立窗口配置
- sw.js：Service Worker 离线缓存
- icons/：192/512 App 图标

## 重要
PWA 的“安装到主屏幕”和 Service Worker 不能在直接双击 `file://` HTML 时完整工作。
需要把整个文件夹放到 HTTPS 网站，或在电脑上用 localhost 运行后访问。
Android Chrome：打开网站 → 浏览器菜单 → 安装应用/添加到主屏幕。
iPhone Safari：打开 HTTPS 网站 → 分享 → 添加到主屏幕。

数据仍由网页自身使用 localStorage / IndexedDB 保存在设备浏览器本地，不需要业务服务器。

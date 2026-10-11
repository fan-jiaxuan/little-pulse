# Little Pulse PWA

中文胎动记录应用。无第三方依赖，记录存储在当前设备的 IndexedDB 中。

## 部署 GitHub Pages
1. 创建公开仓库（例如 `little-pulse`）。
2. 上传本目录中的 **所有文件和 icons 文件夹** 到仓库根目录。
3. Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save。
4. 等待 Pages 部署完成，使用 Safari 打开 `https://用户名.github.io/little-pulse/`。
5. Safari 分享 → 添加到主屏幕。

## 本地测试
在本目录运行 `python3 -m http.server 8000`，访问 `http://localhost:8000`。正式部署需要 HTTPS。

## 说明
- 支持记录、撤销、补录、编辑时间/强度、删除、7/14/30 天趋势、CSV 和 JSON 备份/导入。
- 本版无 iOS 原生 Widget；可将主屏幕图标或快捷指令作为启动入口。
- 浏览器清理网站数据或删除 Web App 可能导致数据丢失。定期导出 JSON 备份。
- 不能通过胎动计数或图表判断胎儿健康。胎动减少或明显变化时应及时联系产科。

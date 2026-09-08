# XLeRobot Home Service Demo — 项目介绍页

对 XLeRobot 稍加改造，完成语音取物递送 Demo，分享参考复现需要的标定、抓取后端、工具、数据和权重。

- [项目实现与文档](https://github.com/xujiayuxian-png/xlerobot_home_service_demo)
- [ACT 权重](https://huggingface.co/lissajous/xlerobot-act-local-grasp-v1)
- [30 条示教数据](https://huggingface.co/datasets/lissajous/xlerobot-glue-stick-grasp-30)

## 本地预览

无需构建，无框架或外部字体依赖：

```bash
python3 -m http.server 8000 --bind 127.0.0.1
```

打开 `http://127.0.0.1:8000`。禁用 JavaScript 时仍可阅读全部内容及使用链接；安全上下文中可复制克隆命令。
本页不连接机器人、ROS 或 GPU 服务。

## 页面内容

真机视频 → ACT 与几何抓取 → 标定工具 → Demo / 建图 / 数采工具 → 参考硬件与复现入口 → 数据与权重。
GitHub Pages 由 `.github/workflows/static.yml` 在 `main` 更新后部署。

`index.html` 包含内容与少量交互；样式在 `assets/site.css`。素材来源和使用边界见 [assets/README.md](assets/README.md)。
技术说明以 Demo 仓库的当前实现为准；软件 replay、拟合残差和独立实测精度不能混为一谈。

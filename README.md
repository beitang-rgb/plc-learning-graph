# PLC 学习图谱 · 工业自动化学习助手

> 覆盖西门子 S7、TIA Portal、Profinet、Modbus、OPC UA、HMI、WinCC 的 PLC 学习知识图谱。
> 含代码示例与学习路径，适合工业软件工程师 / MES 工程师。

## 在线访问

- **GitHub Pages**: https://beitang-rgb.github.io/plc-learning-graph/
- **Cloudflare Pages**（部署后）: https://plc-learning-graph.pages.dev/

## 学习内容

| 阶段 | 内容 | 节点数 |
|------|------|--------|
| 基础 | 电气基础、PLC 概念、IEC 61131-3、变量与数据类型 | 5 |
| 中段 | TIA Portal、LAD/SCL/FBD、FB/FC/OB、DB 数据块、寻址 | 8 |
| 应用 | HMI、Profinet、Modbus、OPC UA | 6 |
| 进阶 | S7-1500、PLCSIM、在线诊断、Python/C# 与 PLC 通信 | 7 |
| 办公型 | MES 数据采集、变频器参数化、WinCC | 5 |

## 代码示例来源

- [OpenPLC](https://github.com/OpenPLC/OpenPLC_v3) - 开源 PLC 运行时
- [beremiz](https://github.com/beremiz/beremiz) - IEC 61131-3 IDE
- [s7netplus](https://github.com/S7NetPlus/s7netplus) - C# S7 通信库
- [pymodbus](https://github.com/pymodbus-dev/pymodbus) - Python Modbus 库
- [snap7](https://github.com/gijzelaerr/python-snap7) - Python S7 通信库

## 技术栈

- D3.js v7 力导向图可视化
- 纯静态 HTML + JS + JSON，零后端依赖
- 支持 GitHub Pages / Cloudflare Pages 部署
- 响应式设计，移动端友好
- SEO 优化：Open Graph / Twitter Card / JSON-LD 结构化数据

## 本地预览

```bash
# 生成站点
python -m graph_engine.learning_web_app --output ./plc_site

# 本地预览
cd plc_site && python -m http.server 8000
```

## 部署

### GitHub Pages（自动部署）
推送到 `main` 分支后，GitHub Actions 会自动部署。

### Cloudflare Pages
```bash
npx wrangler pages deploy . --project-name plc-learning-graph
```

## License

MIT

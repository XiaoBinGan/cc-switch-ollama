# CC Switch Ollama 🦙🐉

基于 [CC Switch v3.16.2](https://github.com/farion1231/cc-switch) 的预编译版本，
**内置 Ollama 本地模型支持**，Codex 可直接使用本地大模型。

## 功能

- ✅ Ollama 供应商预设（开箱即用）
- ✅ Codex Responses → Chat Completions 协议转换
- ✅ Qwen 系列 thinking/reasoning 支持
- ✅ 预置 5 个本地模型，自动识别
- ✅ 修复：健康检查 404 / reasoning.effort 400 / URL 端点丢失

## 下载

| 平台 | 下载 |
|------|------|
| 🍎 macOS (Apple Silicon) | [Releases](../../releases/latest) |
| 🪟 Windows (x64) | [Releases](../../releases/latest) |

## 快速上手

```bash
# 1. 启动 Ollama
ollama serve

# 2. 拉取模型
ollama pull qwen3.5:9b

# 3. 打开 CC Switch Ollama → Codex → 添加供应商 → 选 Ollama (Local)
# 4. 开启本地路由 → 勾选 Codex 接管
# 5. 用 Codex 干活
codex "hello world"
```

## 预置模型

| 模型 | 大小 | 上下文 |
|------|------|--------|
| qwen3.5:9b | 6.6 GB | 128K |
| qwen2.5:14b | 9.0 GB | 128K |
| qwen2.5:7b | 4.7 GB | 128K |
| qwen3:8b | 5.2 GB | 32K |
| gpt-oss:20b | 13.8 GB | 32K |

## 源码

- Fork 分支：<https://github.com/XiaoBinGan/cc-switch/tree/feat/ollama-codex-proxy>
- 上游 PR：<https://github.com/farion1231/cc-switch/pull/4075>

## 许可

继承上游 CC Switch 许可

# RAG-QA-Customer-Service

A RAG-based intelligent Q&A system for customer service scenarios, built with LangChain and DeepSeek.

## 📌 项目简介

本项目是一个基于 RAG（检索增强生成）架构的智能问答系统 POC，以企业售后服务为验证场景。系统通过 LangChain 框架调用 DeepSeek 大模型，结合向量数据库检索，实现对企业知识库的智能问答，并支持用户意图识别、情感分析和优先级分流。

## 🧠 核心功能

- 基于用户问题，从向量数据库中检索相关文档片段
- 调用 DeepSeek 大模型生成自然语言回答
- 支持多格式文档导入（TXT、PDF 等）
- 输出包含用户意图、情感标签和优先级建议

## 🛠️ 技术栈

- LangChain
- DeepSeek API
- HuggingFace Embeddings
- Chroma 向量数据库
- FastAPI
- Python 3.10+

## 🚀 快速开始

```bash
# 1. 克隆仓库
git clone https://github.com/Irene-a11y-kit/RAG-QA-Customer-Service.git

# 2. 安装依赖
pip install -r requirements.txt

# 3. 配置环境变量
# 在项目根目录创建 .env 文件，填入你的 DeepSeek API Key：
# DEEPSEEK_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

# 4. 启动服务
python app.py
```

## 📁 项目结构

```
├── app.py              # FastAPI 主程序
├── requirements.txt    # 项目依赖
├── .env.example        # 环境变量示例
├── knowledge_base/     # 知识库文件存放目录（需自行添加）
└── README.md
```

## 📌 项目状态

当前为 POC 阶段，核心功能已跑通，后续计划：
- 优化 Prompt 模板，提升回答准确性
- 增加对话上下文长度支持
- 接入更多文档格式（Word、Markdown）
- 添加简单的前端交互界面

## 📄 License

MIT License

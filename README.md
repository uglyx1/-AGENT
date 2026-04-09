# 电商运营 Agent（公开展示版）

这是一个面向作品展示与客户沟通的公开版本仓库。

为保护商业机密，仓库仅包含：

- 项目定位与能力说明
- 系统架构与工作流
- API 交互契约（演示级）
- 功能模块与简历描述文档

仓库明确不包含：

- 核心业务源码
- 私有自动化脚本
- 内部策略规则与敏感数据
- 生产环境配置与凭据

## 项目简介

该 Agent 项目面向电商运营场景，核心能力包括：

1. 对话式查询路由（库存 / 市场）
2. 双平台利润对比与报表导出
3. 上架与改价流程草稿编排（Dry-Run）
4. 基于 RAG 的商品检索与 SKU 召回

## 技术方向

- 后端服务：FastAPI 风格的接口架构
- Agent 编排：工具化路由 + 可解释 tool_calls
- 检索系统：Embedding + 向量库 + Rerank + TF-IDF 回退
- 报表能力：结构化结果 + CSV 下载链路
- 前端集成：可通过浏览器脚本或业务面板接入

## 文档结构

- `docs/ARCHITECTURE.md`：系统架构与工作流
- `docs/FEATURES.md`：核心功能模块说明
- `docs/API_CONTRACT.md`：接口契约与请求示例
- `docs/SECURITY_AND_SCOPE.md`：公开范围与保密边界
- `docs/RESUME_DESCRIPTION.md`：可直接复用的项目介绍文案
- `PUBLISH_STEPS.md`：英文上传步骤
- `PUBLISH_STEPS_CN.md`：中文上传步骤

## 说明

该仓库用于展示项目能力，不作为生产交付代码仓库。

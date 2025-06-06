# 法律文档脱敏工具

## 项目概述

法律文档脱敏工具是一个专为法律领域设计的数据脱敏解决方案，旨在保护文档中的敏感信息，同时保持文档的可读性和上下文完整性。该工具能够自动识别并替换文档中的敏感实体（如人名、组织机构、地点、身份证号、电话号码等），使文档可以安全地用于云端LLM服务或公开场合，有效防止隐私泄露。

### 主要功能

- **自动实体识别**：基于先进的NER（命名实体识别）模型，自动识别文本中的敏感实体
- **多种脱敏策略**：支持多种脱敏策略，包括上下文感知替换、类型替换、哈希替换等
- **文档格式支持**：支持PDF、DOC、DOCX、TXT、MD等多种文档格式
- **批量处理**：支持批量处理大量文档，提高工作效率
- **映射表管理**：维护脱敏前后的映射关系，支持文档的恢复功能
- **Web界面**：提供友好的Web界面，方便用户操作和配置
- **API接口**：提供RESTful API接口，便于与其他系统集成

## 文档目录

- [项目架构](./architecture.md)：系统架构设计和模块组织
- [核心模块](./core_modules.md)：核心模块的详细说明
- [脱敏策略](./masking_strategies.md)：各种脱敏策略的实现和使用
- [API文档](./api_reference.md)：API接口的详细说明
- [使用指南](./user_guide.md)：系统使用方法和最佳实践
- [部署说明](./deployment.md)：系统部署和配置指南

## 技术栈

- **后端**：Python、Flask
- **NER模型**：ModelScope NLP RANER 中文命名实体识别模型
- **文档处理**：支持多种文档格式的解析和转换
- **前端**：HTML、CSS、JavaScript、Bootstrap

## 快速开始

1. 安装依赖：
   ```bash
   pip install -r requirements.txt
   ```

2. 启动Web服务：
   ```bash
   python -m Data_Masking.ui.app
   ```

3. 访问Web界面：
   ```
   http://localhost:8080
   ```

## 许可证

本项目采用 [MIT 许可证](LICENSE)。
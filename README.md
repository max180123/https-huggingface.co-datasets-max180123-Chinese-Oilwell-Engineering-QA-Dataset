# 中文油气井工程问答数据集（Chinese-Oilwell-Engineering-QA-Dataset）

本数据集面向油气井工程场景，聚焦钻井工程、完井工程、井壁稳定与石油工程导论等核心知识，采用问答（QA）形式组织，适用于中文技术领域大模型的指令对齐与领域微调。

<p align="center">
🤗 <a href="https://huggingface.co/datasets/max180123/Chinese-Oilwell-Engineering-QA-Dataset">Hugging Face</a>&nbsp&nbsp | &nbsp&nbsp🤖 <a href="https://modelscope.cn/datasets/max0123/Chinese-Oilwell-Engineering-QA-Dataset">ModelScope</a>&nbsp&nbsp | &nbsp&nbsp🚀 <a href="https://github.com/max180123/https-huggingface.co-datasets-max180123-Chinese-Oilwell-Engineering-QA-Dataset">GitHub</a>
</p>

## 数据集概览

- **规模**：共 19,355 条样本（统计脚本见下）。
- **类型**：QA 型（基于 `instruction` → `output` 的指令问答结构）。
- **格式**：JSON 数组（`json-array`）。
- **领域**：钻井工程、完井工程、井壁稳定、石油工程导论等。


## 数据来源与整理

本数据集主要依据以下来源进行整理与归纳：

- 钻井工程、完井工程、井壁稳定、石油工程导论等相关教材与专著
- 公开的综述性学术文献与工程实践资料

在整理过程中，我们进行了人工初步查验与审核，以提升数据的一致性与可用性；但鉴于专业领域广度与复杂性，仍建议在实际工程应用前结合现场经验进行复核。

## 数据格式

数据采用 JSON 数组存储，每个样本为一个对象，核心字段如下：

- `instruction`: 指令/问题（字符串，必有）
- `input`: 可选输入（字符串，可为空）
- `output`: 回答/解答（字符串，必有）
- `system`: 可选系统提示（字符串，可为空）

数据示例：

```json
{
  "instruction": "井壁稳定的定义是什么？",
  "input": "",
  "output": "井壁稳定是指在钻井过程中，通过钻井液密度、钻井液体系和钻井工艺三者的协同作用，确保井眼不坍塌、不破裂、不缩径的状态……",
  "system": ""
}
```

## 预期用途

- 中文技术领域 LLM 的指令微调（SFT）
- 专业问答系统、检索增强问答（RAG）原型验证
- 井工程知识图谱构建与评测数据

## 局限性与免责说明

尽管本数据集经过人工初步查验与审核，整体质量较高，但仍存在以下局限：

- 可能存在个别表述不够严谨或与最新行业实践不完全一致的情况；
- 复杂工况下的工程参数需结合现场实测和规范要求进行二次校核；
- 数据并不构成工程设计或安全决策的直接依据。

因此，使用者应自行甄别并承担使用风险。因使用本数据集导致的任何直接或间接损失、纠纷或安全事故，数据集作者与维护者不承担任何责任。


## 许可证

本项目采用 Apache License 2.0 许可证。

## 引用

若本数据集对您的研究或产品有帮助，请引用：

```text
@misc{Chinese-Oilwell-Engineering-QA-Dataset,
  author    = {Ning Li , Xueqiang Ma , Saina Yue , Quan Zhang , Bao Zhou , Menghan Si , Jinlu Liu},
  title     = {Chinese Oilwell Engineering QA Dataset},
  year      = {2025},
  publisher = {GitHub},
  howpublished = { \url{https://github.com/max180123/https-huggingface.co-datasets-max180123-Chinese-Oilwell-Engineering-QA-Dataset}},
}
```

## 联系作者

- Email: ma180123@163.com



---
description: ListOutput 节点操作指南
---

# 列表渲染

***

## 图示

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

***

## 简介

ListOutput 节点是用于处理列表输出的工作流节点组件。它接收输入列表，并将其按指定分隔符连接成字符串，然后将结果传递到下一个节点。

## 参数详解

* **list (List\<String>)**: 必填参数，表示待处理的输入列表。
* **splitter (String)**: 必填参数，表示用于连接列表元素的分隔符。
* **output (String)**: 输出参数，表示处理后的输出字符串。

## 使用方法

1. **配置节点参数**: 在节点配置界面中，填写待处理的输入列表到参数 `list` 中，并指定连接列表元素的分隔符到参数 `splitter` 中。
2. **执行节点**: 执行 ListOutput 节点，以处理输入列表，并将连接后的结果传递到下一个节点。

## 使用示例

假设有以下输入数据：

```java
"apple", "banana", "orange"
```

执行 ListOutput 节点后，输出结果为：

```json
{
  "list": ["apple", "banana", "orange"],
  "splitter": ",",
  "output": "apple,banana,orange"
}
```

以上示例展示了使用 ListOutput 节点进行列表输出处理的过程。输入数据包含待处理的列表和分隔符，输出结果是连接后的字符串。

## 注意事项

* 请确保参数 `list` 和 `splitter` 的值有效，并符合您的业务需求。
* 分隔符 `splitter` 可以是单个字符，也可以是多个字符的组合。

***


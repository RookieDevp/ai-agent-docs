---
description: TextInput 节点操作指南
---

# 文本输入

***

## 图示

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

***

## 简介

TextInput 节点是用于处理文本输入的工作流节点组件。它接收输入字符串，并将其传递到下一个节点。

## 参数详解

* **inputStr (String)**: 必填参数，表示待处理的输入字符串。

## 输出类型

输出类型为字符串，是输入字符串经过处理后的结果。

## 使用方法

1. **配置节点参数**: 在节点配置界面中，填写待处理的输入字符串到参数 `inputStr` 中。
2. **执行节点**: 执行 TextInput 节点，以处理输入字符串，并将结果传递到下一个节点。

## 使用示例

假设有以下输入数据：

```java
"Hello, world!"
```

执行 TextInput 节点后，输出结果为：

```json
{
  "output": "Hello, world!"
}
```

以上示例展示了使用 TextInput 节点进行文本输入处理的过程。输入数据包含待处理的输入字符串，输出结果是处理后的字符串。

## 注意事项

* 请确保参数 `inputStr` 的值有效，并符合您的业务需求。

***


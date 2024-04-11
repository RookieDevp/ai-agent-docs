---
description: TextSegmentation 节点操作指南
---

# 文本分割

***

## **图示**

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

***

## **简介**

TextSegmentation 节点是用于文本分割的工作流节点组件。它能够根据指定的分隔符，将输入的文本字符串分割成多个子串，并输出分割后的结果。

***

## **参数详解**

* **text (String)**: 必填参数，表示待分割的文本字符串。
* **splitter (String)**: 必填参数，表示用于分割文本的分隔符。

***

## **输出类型**

输出类型为列表，包含根据分隔符分割后得到的子串列表。

***

## **使用方法**

1. **配置节点参数**: 在节点配置界面中，填写待分割的文本字符串到参数 `text` 中，并指定分隔符到参数 `splitter` 中。
2. **执行节点**: 执行 TextSegmentation 节点，以生成分割后的子串列表。

***

## **使用示例**

假设有以下输入数据：

```json
{
  "text": "apple,banana,orange",
  "splitter": ","
}
```

执行 TextSegmentation 节点后，输出结果为：

```json
[
  "apple",
  "banana",
  "orange"
]
```

以上示例展示了使用 TextSegmentation 节点进行文本分割的过程。输入数据包含待分割的文本字符串和分隔符，输出结果是根据分隔符分割后的子串列表。

***

## **注意事项**

* 请确保参数 `text` 和 `splitter` 的值有效，并符合您的业务需求。
* 分隔符 `splitter` 可以是单个字符，也可以是多个字符的组合。

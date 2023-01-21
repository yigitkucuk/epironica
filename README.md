---
tags:
- text-classification
language:
- en
widget:
- text: "Your text here"
datasets:
- yigitkucuk/autotrain-data-row-eval
---

# Model

- Problem type: Multi-class Classification
- Model ID: 2994886333

## Validation Metrics

- Loss: 0.537
- Accuracy: 0.721
- Macro F1: 0.720
- Micro F1: 0.721
- Weighted F1: 0.720
- Macro Precision: 0.723
- Micro Precision: 0.721
- Weighted Precision: 0.723
- Macro Recall: 0.721
- Micro Recall: 0.721
- Weighted Recall: 0.721


## Usage

You can use cURL to access this model:

```
$ curl -X POST -H "Authorization: Bearer YOUR_API_KEY" -H "Content-Type: application/json" -d '{"inputs": "Your text here"}' https://api-inference.huggingface.co/models/yigitkucuk/Not-My-Hat
```

Or Python API:

```
from transformers import AutoModelForSequenceClassification, AutoTokenizer

model = AutoModelForSequenceClassification.from_pretrained("yigitkucuk/Not-My-Hat", use_auth_token=True)

tokenizer = AutoTokenizer.from_pretrained("yigitkucuk/Not-My-Hat", use_auth_token=True)

inputs = tokenizer("Your text here", return_tensors="pt")

outputs = model(**inputs)
```

## Reach This Model on Huggingface

https://huggingface.co/yigitkucuk/Not-My-Hat

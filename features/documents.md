# Documents

With Whitehead NLU, you can also integrate it with your document storage on most cloud storage providers like AWS S3, Dropbox, Google Drive, Google Cloud Storage etc. to extend NLU training abilities to them.

## answer ![private-preview](../.gitbook/assets/private-preview-text.png)

> [Join the waitlist](https://roadmap.whitehead.ai/16)

Answer plain-language questions from a given context, including a set of documents.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | yes |

**Signature:**

```python
context: str = """
(Nikola_Tesla) On his 50th birthday in 1906, Tesla demonstrated his 200 horsepower (150 kilowatts) 16,000 rpm bladeless turbine.
"""

question: str = "At what speed did the turbine operate?"

result: str = await answer(question, context)
# --> 16,000 rpm

# -----------------------------
# Using a custom model
# -----------------------------

model_id: str

result = await answer("What is the return policy?", model_id=model_id)
```

## search ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/18)

Semantic search and retrieval of queries from a set of documents.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| no | yes |

**Signature:**

```python
<UNDECIDED>
```

## summarize ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/17)

Summarize document or passage. Zero-shot, no custom training required.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
<UNDECIDED>
```


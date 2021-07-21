# Utilities

Utilities for common NLU tasks like preprocessing and generating grammatically correct sentences from data.

## template ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/24)

Generate output by interpolating variables in templates and apply the correct tense and inflections.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
# We commonly find ourselves knowing what verb to suggest, but not what conjugation...
options = {
  "some_verb": "looks"
}

input = "Why John, you're {some_verb} handsome today!"

result = await template(input, options)
# >>> "Why John, you're looking handsome today!"
```

## normalize ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/23)

Normalize input to remove spelling mistakes, common grammatical mistakes etc.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
input: str = "These phones is nt gud"

result: str = await normalize(input)
# >>> "These phones are not good"
```


# Understanding

Whitehead Natural Language tools not only enable you to analyze text but also reason over them, apply commonsense, and understand its meaning.

## sensibility ![private-preview](../.gitbook/assets/private-preview-text.png)

> [Join the waitlist](http://fill-this-form)

Rank a list of inputs according to how sensible they are in a given context.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
context: str = "I am interested in finding out about different courses"
candidates: List[str] = [
  "He is a great basketball player.",
  "We offer three different biology courses. You can find out more on them from our website",
]

result: List[Tuple[str, float]] = await sensibility(candidates, context)
# >>> [
  ("He is a great basketball player.", 0.02),
  ("We offer three different biology courses. You can find out more on them from our website", 0.71),
]
```

## deduce ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Apply commonsense reasoning to normal situation.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
input: str = "Making hot tea"

first_steps: List[str] = await deduce(input, HasFirstSubevent)
# >>> [
#   "Boil water",
#   "Heat stove",
# ... ]
```

## topics ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Mine topics from a given input.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | yes |

**Signature:**

```python
input: str = "I went to Canada and brought back a dozen macintosh apples"
topics: List[str] = ["food", "computers",  "travel", "technology"]

result: List[Tuple[str, float]] = await topics(input, topics)
# >>> [
#   ("food", 0.76),
#   ("computers", 0.13),
# .... ]
```

## smartcomplete ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29%20%281%29.png)

> [Join the waitlist](http://fill-this-form)

Smart auto-completion of a user prompt.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
input: str = "Hey John, unfortunately I am not available today or tomorrow but are you free on"
context: str = "Today is Monday."

result: str = await smartcomplete(input, context)
# >>> "Wednesday or Thursday?"
```


# Conversations

Natural language understanding tools that makes it easy to design and integrate a conversational user interface into your mobile app, web application, device, bot, interactive voice response system, and so on

## intent ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/15)

Train utterances against an intent classifier to recognize user intent from new inputs. Can also be used in a zero-shot configuration to intents in plain English.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| no | yes |

**Signature:**

```python
model_id: str
input: str = "It's raining today but ideally I would love to order a pizza"

result: str = await intent(input, model_id=model_id)
# >>> "order_pizza"
```

## match ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/14)

Match user input against a predefined template to extract "slot" values.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
<UNDECIDED>
```

## chitchat ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Conduct free-form chit-chat with your users.

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | yes |

**Signature:**

```python
input: str
history = [
  {"user": str},
  {"bot": str}, ... ]

result = await chitchat(input, history)
# >>> Wassup!
```

## dialogact ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/13)

Tag dialog utterances with [_dialog acts_](https://en.wikipedia.org/wiki/Dialog_act)_._

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | no |

**Signature:**

```python
input: str

history = [
  {"user": str},
  {"bot": str}, ... ]

result: str = await dialogact(input, history)
# >>> Wh-Question
```


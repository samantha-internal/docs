# Speech

Convert text into natural-sounding speech and back. Or train model to identify speakers based on previously recorded speech.

## speak ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Convert text to natural-sounding speech

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | yes |

**Signature:**

```python
result: BinaryIO[bytes] = await speak(sentence)
# returns a stream
```

## transcribe ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Transcribe speech audio to extract text

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| yes | yes |

**Signature:**

```python
input: BinaryIO[bytes]

result: str = await transcribe(input)
```

## identify ![coming-soon](../.gitbook/assets/coming-soon-text%20%281%29.png)

> [Join the waitlist](https://roadmap.whitehead.ai/11)

Identify speakers from speech audio

| Zero-shot \(ready to use\) | Trainable |
| :--- | :--- |
| no | no |

**Signature:**

```python
<UNDECIDED>
```


# Compose

Perhaps the most powerful feature of the Whitehead AI platform, `compose` lets you create arbitrary solutions for your use case by composing different APIs together in custom pipelines. You can create them on the fly and unlike calling them step-by-step, the entire inference happens in one request optimized for latency. 

## compose ![beta](../.gitbook/assets/beta-text%20%281%29.png)

Easily compose different Whitehead APIs together in a single inference pipeline.

**Signature:**

```python
# use case: speech-based semantic search
speech_search = compose([
  transcribe,
  search(..., model_id=1234),
  speak
])

result = await speech_search(audio)

# -------------------------------

# use case: gmail-like autocomplete using pre-trained search model
autocomplete = compose([
  search(model_id),
  smartcomplete
])

result = await autocomplete(input)
```


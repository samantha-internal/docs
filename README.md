# Introduction

## NLU for humans.

Whitehead is a simple and elegant API for common natural language tasks. You can use them to build games, chatbots, and novel conversational interfaces. Features include:

* Freeform chit-chat with users
* Generating natural-sounding speech
* Understanding user intent and extracting information
* Among [many others](content/concepts/untitled.md)...

## Wonderfully simple and tasteful libraries

Whitehead libraries have been designed for human beings. They are simple and high-level so you can focus on the design and "feel" of your applications rather than the technical details. You can see for yourself in these examples!

{% tabs %}
{% tab title="node.js" %}
{% code title="hello.js" %}
```javascript
/* Assuming you already have a `client` instance ready. */

/* Example 1: Get a response to a chitchat message */
// > See API reference for a list of all of our APIs
const input = "It is a good day today";
const history = [
  {agent: "user", said: "Hello"},
  {agent: "bot", said: "Hi there!"}
];

const result = await client.api.chitchat({ input, history });

/*
  {reply: "It's been nice for a few days now."}
*/

// --------------------------------------------

```
{% endcode %}
{% endtab %}

{% tab title="python" %}
{% code title="hello.py" %}
```python
# Assuming you already have a `client` instance ready.

from whitehead_sdk.api.input.turn import Turn, Agent

# Example 1: Get a response to a chitchat message
# > See API reference for a list of all APIs
result = client.chitchat.execute( 
    input="It is a good day today", 
    history=[
        Turn(agent=Agent.USER, said="Hello"),
        Turn(agent=Agent.BOT, said="Hi there")
    ]
)

# {
#   "reply": "It's been beautiful for a few days now."
# }

# ----------------------------------------------------

```
{% endcode %}
{% endtab %}
{% endtabs %}




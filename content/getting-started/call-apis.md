# Call APIs

## Start calling our APIs

After creating an authenticated client from [the previous step](setup-client.md#authenticate-and-start-session), you are ready to start calling our APIs! Here are some example queries that you can try:

{% hint style="warning" %}
**Heads up!** These examples are incomplete without the previous step for the sake of clarity and cannot be run as is.
{% endhint %}

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




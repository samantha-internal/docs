# Call APIs

## Authenticate and start session

Once you have the SDK package installed, you can directly use the credentials obtained in [the previous step](get-api-key.md#grab-your-id-and-private-key) to authenticate your session and start using the API.

{% hint style="info" %}
For authentication, the `Whitehead` constructor searches for credentials in the following order:

1. The `developer_id` and `api_key` parameters passed.  
2. Environment variables `WHITEHEAD_DEVELOPER_ID` and `WHITEHEAD_API_KEY`  
3. Access token, if persisted, from `~/.cache/whitehead/access-token` \(This only stores the generated access token and not the plain api key\)  
{% endhint %}

{% tabs %}
{% tab title="node.js" %}
```javascript
import { authenticate, chitchat, answer, smartcomplete, paraphrase } from "@whitehead/sdk";

// Or, for commonjs:
// const { authenticate, chitchat, answer, smartcomplete, paraphrase } = require("@whitehead/sdk");

async function call_apis() {
    // Credentials optional if the tokens were saved locally by running
    // the CLI `whitehead login` command beforehand
    await authenticate({api_key: "XXXXXXXXXXXXXXXXXX", developer_id: 42})

    let result;
    result = await chitchat("Which TV actor do you like?");
    // "I don't really like watching TV but I kinda like Jennifer Aniston."

    result = await answer(
      "Where did John go?",
      {context: "John and Mary went to Brighton Beach for their honeymoon."}
    )
    // {
    //   "answer": "You can take 5 days off every quarter as a paid leave.",
    //   "reference": {...}
    // }

    result = await smartcomplete(
      "Dear Martha, I am not free today but would you like to grab coffee on", 
      {context: "Today is Monday."}
    )
    // "Tuesday or Wednesday?",

    result = await paraphrase("Can I have a large pizza?")
    // [
    //   "I would like to have a large pizza",
    //   ...
    // ]

}
```
{% endtab %}

{% tab title="Python3 \(async\)" %}
```python
from whitehead import *

async def call_apis():
    # Credentials optional if the tokens were saved locally by running
    # the CLI `whitehead login` command beforehand
    await authenticate(api_key="XXXXXXXXXXXXXXXXXX", developer_id=42)

    result = await chitchat("Which TV actor do you like?")
    # "I don't really like watching TV but I kinda like Jennifer Aniston."

    result = await answer(
        "Where did John go?",
        context="John and Mary went to Brighton Beach for their honeymoon.")
    # {
    #   "answer": "You can take 5 days off every quarter as a paid leave.",
    #   "reference": {...}
    # }

    result = await smartcomplete(
        "Dear Martha, I am not free today but would you like to grab coffee on", 
        context="Today is Monday.")
    # "Tuesday or Wednesday?",

    result = await paraphrase("Can I have a large pizza?")
    # [
    #   "I would like to have a large pizza",
    #   ...
    # ]
```
{% endtab %}

{% tab title="Python3 \(sync\)" %}
```python
from whitehead.sync import *

# NOT RECOMMENDED unless not convenient to use the async API

def call_apis():
    # Credentials optional if the tokens were saved locally by running
    # the CLI `whitehead login` command beforehand
    authenticate(api_key="XXXXXXXXXXXXXXXXXX", developer_id=42)

    result = chitchat("Which TV actor do you like?")
    # "I don't really like watching TV but I kinda like Jennifer Aniston."

    result = answer(
        "Where did John go?",
        context="John and Mary went to Brighton Beach for their honeymoon.")
    # {
    #   "answer": "You can take 5 days off every quarter as a paid leave.",
    #   "reference": {...}
    # }

    result = smartcomplete(
        "Dear Martha, I am not free today but would you like to grab coffee on", 
        context="Today is Monday.")
    # "Tuesday or Wednesday?",

    result = paraphrase("Can I have a large pizza?")
    # [
    #   "I would like to have a large pizza",
    #   ...
    # ]
```
{% endtab %}
{% endtabs %}


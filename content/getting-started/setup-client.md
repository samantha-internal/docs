# Setup client

## Install the SDK

Install the _Whitehead SDK_ in your favorite runtime \(we currently support `node.js 8.0+` and `python 3.5+`\):

{% tabs %}
{% tab title="node.js" %}
```bash
# Install using npm
npm install @whitehead/sdk
```
{% endtab %}

{% tab title="python" %}
```bash
# Install using pip
pip install whitehead-sdk

# Or poetry
poetry add whitehead-sdk
```
{% endtab %}
{% endtabs %}

> If you encountered an error during the installation, please report the issue on the sdk repo [for node](https://github.com/whitehead-ai/node-sdk/issues) or [for python](https://github.com/whitehead-ai/python-sdk/issues) respectively.

## Authenticate and start session

Once you have the SDK package installed, you can directly use the credentials obtained in [the previous step](get-api-key.md#grab-your-id-and-private-key) to authenticate your session and start using the API.

{% tabs %}
{% tab title="node.js" %}
{% code title="hello.js" %}
```javascript
const { Whitehead } = require("@whitehead/sdk");

// ES6 modules: import Whitehead from "@whitehead/sdk/esm";
// Typescript: import Whitehead from "@whitehead/sdk/ts";

// Credentials from the previous step
const developerId = 42;
const apiKey = "<64 letter api key from your mauna dashboard>";

// Instantiate client
const client = new Whitehead(developerId, apiKey);

/* Great! Now you can start calling APIs. :) */

```
{% endcode %}
{% endtab %}

{% tab title="python" %}
{% code title="hello.py" %}
```python
from whitehead_sdk import Whitehead

# Credentials from the previous step
developer_id = 42
api_key = "<64 letter api key available on your mauna dashboard>"

# Instantiate client
client = Whitehead(developer_id, api_key)

# Great! Now you can start calling APIs. :)

```
{% endcode %}
{% endtab %}
{% endtabs %}

{% hint style="info" %}

For authentication, the `Whitehead` constructor searches for credentials in the following order:
1. The `developer_id` and `api_key` parameters passed.
2. Environment variables `WHITEHEAD_DEVELOPER_ID` and `WHITEHEAD_API_KEY`
3. Access token, if persisted, from `~/.cache/whitehead/access-token` (This only stores the generated access token and not the plain api key)

{% endhint %}

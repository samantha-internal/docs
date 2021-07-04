# Introduction

## Whitehead: NLU and Conv AI for humans.

Whitehead is a simple and elegant **API** for common natural language tasks needed by conversational interfaces. For example,

 - Free form chit-chat with users
 - Generating natural-sounding speech
 - Understanding user intent and extracting information
 - Among [many others](content/list-of-features.md)...

## Wonderfully simple and tasteful libraries.

The Whitehead libraries have been designed for human beings. They are simple and high-level so you can focus on the design and "feel" of your applications rather than the technical details. You can see for yourself in these examples!

{% tabs }

{% tab title="Chit-chat" }
{% code }

``` python
await chitchat("Which TV actor do you like?")
# "I don't really like watching TV but I kinda like Jennifer Aniston."

```

{% endcode }
{% endtab }

{% tab title="Answer questions" }
{% code }

``` python

# The context can be a plain string passage as well.
await answer(
    "How many days paid leave can I take?",
    context="https://www.dropbox.com/s/xxxxxxxxxxx/HR_handbook.pdf")

# {
#   "answer": "You can take 5 days off every quarter as a paid leave.",
#   "reference": {
#     "url": "https://www.dropbox.com/s/xxxxxxxxxxx/HR_handbook.pdf",
#     "location": [124, 125, 126]
#   }
# }

```

{% endcode }
{% endtab }

{% tab title="Smartcomplete" }
{% code }

``` python

await smartcomplete(
    "Dear Martha, I am not free today but would you like to grab coffee on", 
    context="Today is Monday.")

# "Tuesday or Wednesday?",

```

{% endcode }
{% endtab }

{% tab title="Transcribe" }
{% code }

``` python

# Works the same with file uploads and URLs
# Automatically updates sampling as needed
await transcribe(websocket.Stream("wss://some-user-input"))

# Iterator<[
#   "I am sorry I did that to you on your wedding day",
#   "but the diarrhea was relentless."
# ]

```

{% endcode }
{% endtab }

{% tab title="Paraphrase" }
{% code }

``` python

await paraphrase("Can I have a large pizza?")

# [
#   "I would like to have a large pizza",
#   "I want a large pizza",
#   "Can you give me a large pizza?",
#   ...
# ]

```

{% endcode }
{% endtab }

{% endtabs }

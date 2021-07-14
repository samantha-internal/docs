# Features

{% hint style="warning" %}
As part of the upgrade to [v0.2](https://docs.whitehead.ai/v/v0.2-preview), a number of APIs are now deprecated for direct use. These have been striked-through below. They will be available for use for existing clients until they are able to migrate to the new version.
{% endhint %}

## Language

| API | Description |
| :--- | :--- |
| `paraphrase sentence` | Generate different ways of saying the same thing, preserving the meaning. |
| `sentiment analysis` | Calculate polarity of a given sentence as a floating point number between `-1` and `1` |
| `measure similarity` | Calculate similarity between a sentence and candidates |
| ~~_nlu_~~ | ~~_Extract entities, vectors and dependencies in a sentence_~~ |
| ~~_resolve coreference_~~ | ~~_Resolve coreferences in a sentence_~~ |

## Speech

| API | Description |
| :--- | :--- |
| `text to speech` | Convert text to natural-sounding speech |
| `speech to text` | Transcribe speech audio to extract text |
| ~~_apply voice css_~~ | ~~_Apply styling to voice using voice css_~~ |

## Conversations

| API | Description |
| :--- | :--- |
| `qa` | Free form and multiple choice question answering on given context |
| `chitchat` | Conduct free-form chit-chat with your users |
| ~~_next dialog turn_~~ | ~~_Predict next turn in a dialog given history_~~ |
| ~~_match intent_~~ | ~~_Parse user input to understand intent and entities_~~ |

## Understanding

| API | Description |
| :--- | :--- |
| `classify topic` | Mine topics from a given input |
| `predict relation` | Predict target objects on the conceptnet graph given subject and relation |
| ~~_parse context_~~ | ~~_Parse an input sentence into its frame-semantics representation_~~ |
| ~~_parse ace_~~ | ~~_Parse an ACE sentence into DRS \(Discourse Representation Structure\)_~~ |
| ~~_commonsense_~~ | ~~_Apply commonsense reasoning to normal situation_~~ |

## Compose

| API | Description |
| :--- | :--- |
| `compose` | Easily compose different Whitehead APIs together in a single inference pipeline |


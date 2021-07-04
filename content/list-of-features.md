# List of features 

## Language

| API          | Description                                                                            |
|:-------------|:---------------------------------------------------------------------------------------|
| `paraphrase` | Generate different ways of saying the same thing, preserving the meaning.              |
| `sentiment`  | Calculate polarity of a given sentence as a floating point number between `-1` and `1` |
| `emotions`   | Classify input by different emotions like, `happiness`, `anger` etc                    |
| `similarity` | Calculate similarity between a sentence and candidates                                 |

## Speech

| API          | Description                             |
|:-------------|:----------------------------------------|
| `speak`      | Convert text to natural-sounding speech |
| `transcribe` | Transcribe speech audio to extract text |
| `identify`   | Identify speakers from speech audio     |

## Conversations

| API         | Description                                                                          |
|:------------|:-------------------------------------------------------------------------------------|
| `parse`     | Parse user input to understand intent and entities                                   |
| `chitchat`  | Conduct free-form chit-chat with your users                                          |
| `dialogtag` | Tag dialog utterances with [_dialog acts_](https://en.wikipedia.org/wiki/Dialog_act) |

## Understanding

| API             | Description                                                                 |
|:----------------|:----------------------------------------------------------------------------|
| `sensibility`   | Rank a list of inputs according to how sensible they are in a given context |
| `deduce`        | Apply commonsense reasoning to normal situation                             |
| `topics`        | Mine topics from a given input                                              |
| `smartcomplete` | Smart auto-completion of a user prompt                                      |
| `entities`      | Extract entities from a given input                                         |

## Documents

| API         | Description                                                                        |
|:------------|:-----------------------------------------------------------------------------------|
| `answer`    | Answer plain-language questions from a given context, including a set of documents |
| `search`    | Semantic search and retrieval of queries from a set of documents                   |
| `summarize` | Summarize document or passage                                                      |

## Compose

| API       | Description                                                                     |
|:----------|:--------------------------------------------------------------------------------|
| `compose` | Easily compose different Whitehead APIs together in a single inference pipeline |

## Training

| API     | Description                                                     |
|:--------|:----------------------------------------------------------------|
| `train` | Train (or more precisely, fine-tune) a task to your own dataset |
| `eval`  | Evaluate accuracy of a custom model for a particular task       |

## Utilities

| API         | Description                                                                                         |
|:------------|:----------------------------------------------------------------------------------------------------|
| `template`  | Generate output by interpolating variables in templates and apply the correct tense and inflections |
| `normalize` | Normalize input to remove spelling mistakes, common grammatical mistakes etc                        |


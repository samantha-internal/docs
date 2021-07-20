# List of features

## Language

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `paraphrase` | Generate different ways of saying the same thing, preserving the meaning. | yes | no |
| `sentiment` | Calculate polarity of a given sentence as a floating point number between `-1` and `1` | yes | yes |
| `emotions` | Classify input by different emotions like, `happiness`, `anger` etc | yes | yes |
| `similarity` | Calculate similarity between a sentence and candidates | yes | no |

## Speech

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `speak` | Convert text to natural-sounding speech | yes | yes |
| `transcribe` | Transcribe speech audio to extract text | yes | yes |
| `identify` | Identify speakers from speech audio | no | yes |

## Conversations

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `intent` | Classify utterances to recognize user intent from new inputs | no | yes |
| `match` | Match user input against a predefined template to extract "slot" values | yes | no |
| `chitchat` | Conduct free-form chit-chat with your users | yes | yes |
| `dialogact` | Tag dialog utterances with [_dialog acts_](https://en.wikipedia.org/wiki/Dialog_act) | yes | no |

## Understanding

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `sensibility` | Rank a list of inputs according to how sensible they are in a given context | yes | no |
| `deduce` | Apply commonsense reasoning to normal situation | yes | no |
| `topics` | Mine topics from a given input | yes | yes |
| `smartcomplete` | Smart auto-completion of a user prompt | yes | no |

## Documents

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `answer` | Answer plain-language questions from a given context, including a set of documents | yes | yes |
| `search` | Semantic search and retrieval of queries from a set of documents | no | yes |
| `summarize` | Summarize document or passage | yes | no |

## Compose

| API | Description |
| :--- | :--- |
| `compose` | Easily compose different Whitehead APIs together in a single inference pipeline |

## Training

| API | Description |
| :--- | :--- |
| `train` | Train \(or more precisely, fine-tune\) a task to your own dataset |
| `eval` | Evaluate accuracy of a custom model for a particular task |

## Utilities

| API | Description | Ready to use | Trainable |
| :--- | :--- | :--- | :--- |
| `template` | Generate output by interpolating variables in templates and apply the correct tense and inflections | yes | no |
| `normalize` | Normalize input to remove spelling mistakes, common grammatical mistakes etc | yes | no |


# query_root

## apps

> An array relationship

**Type:** [`[apps!]!`](objects.md#apps)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[apps_select_column!]`](enums.md#apps_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[apps_order_by!]`](inputs.md#apps_order_by) | sort the rows by one or more columns |  |
| `where` | [`apps_bool_exp`](inputs.md#apps_bool_exp) | filter the rows returned |  |

## atomic_data

> fetch data from the table: "atomic.data"

**Type:** [`[atomic_data!]!`](objects.md#atomic_data)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[atomic_data_select_column!]`](enums.md#atomic_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[atomic_data_order_by!]`](inputs.md#atomic_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`atomic_data_bool_exp`](inputs.md#atomic_data_bool_exp) | filter the rows returned |  |

## atomic_data_aggregate

> fetch aggregated fields from the table: "atomic.data"

**Type:** [`atomic_data_aggregate!`](objects.md#atomic_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[atomic_data_select_column!]`](enums.md#atomic_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[atomic_data_order_by!]`](inputs.md#atomic_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`atomic_data_bool_exp`](inputs.md#atomic_data_bool_exp) | filter the rows returned |  |

## callApplyVoiceCSS

> Apply voice CSS to the SSML input

**Type:** [`SSMLResult`](objects.md#ssmlresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `styled_ssml` | [`String`](scalars.md#string) |  |  |
| `voice_css` | [`String`](scalars.md#string) |  |  |

## callChitchat

> Perform chit chat

**Type:** [`ChitchatResponse`](objects.md#chitchatresponse)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `history` | [`[Turn!]`](inputs.md#turn) |  |  |
| `input` | [`String`](scalars.md#string) |  |  |

## callClassifyTopic

> Classify topics

**Type:** [`ClassificationResult`](objects.md#classificationresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `allow_multiple` | [`Boolean`](scalars.md#boolean) | Allow multiple topics to be applicable | `false` |
| `input` | [`String!`](scalars.md#string) |  |  |
| `topics` | [`[String!]`](scalars.md#string) |  |  |

## callCommonsense

> Predict category

**Type:** [`RelationResult`](objects.md#relationresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `category` | [`Category`](enums.md#category) | Category to extract from input | `null` |
| `input` | [`String!`](scalars.md#string) | Text string |  |

## callCompose

> Execute composition pipeline

**Type:** [`ComposeResult`](objects.md#composeresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `init` | [`JSON`](scalars.md#json) |  |  |
| `pipeline` | [`[InputPipe]!`](inputs.md#inputpipe) |  |  |

## callMatchIntent

> Call the intent matching functionality

**Type:** [`MatchIntentOutput`](objects.md#matchintentoutput)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String`](scalars.md#string) |  | `null` |
| `possible_intents` | [`[String]`](scalars.md#string) |  | `null` |
| `similarity_threshold` | [`Float`](scalars.md#float) |  | `0.8` |

## callMeasureSimilarity

> Measure sentences similarity

**Type:** [`SentenceSimilarityScores`](objects.md#sentencesimilarityscores)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `candidates` | [`[String]`](scalars.md#string) |  |  |
| `input` | [`String`](scalars.md#string) |  |  |

## callNLU

> Document processing

**Type:** [`NLUResult`](objects.md#nluresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String!`](scalars.md#string) | Text to perform NLU tasks on |  |

## callNextDialogTurn

> Perform next dialog turn prediction

**Type:** [`Result`](objects.md#result)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `history` | [`[Turn!]`](inputs.md#turn) | Utterances history |  |
| `input` | [`[String]`](scalars.md#string) | Alternatives to choose from |  |

## callParaphraseSentence

> Perform sentence paraphrasing

**Type:** [`Paraphrase`](objects.md#paraphrase)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String`](scalars.md#string) |  |  |

## callParseACE

> Parse ACE sentence

**Type:** [`ACEResult`](objects.md#aceresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `format` | [`ACEOutputType`](enums.md#aceoutputtype) |  |  |
| `guess` | [`Boolean`](scalars.md#boolean) |  |  |
| `text` | [`String!`](scalars.md#string) |  |  |

## callParseContext

> Parse frame semantics for a list of dialog turns

**Type:** [`[ContextResult]`](objects.md#contextresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `turns` | [`[ContextObject]`](inputs.md#contextobject) | List of possible turns |  |

## callPredictRelation

> Predict relations

**Type:** [`RelationResult`](objects.md#relationresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String!`](scalars.md#string) | Text string |  |
| `relation` | [`Relation`](enums.md#relation) | Relation to extract from input | `null` |

## callQA

> Answer questions based on context

**Type:** [`QA_Result`](objects.md#qa_result)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `choices` | [`[String]`](scalars.md#string) | Alternatives to choose answer from | `[]` |
| `context` | [`String!`](scalars.md#string) |  |  |
| `input` | [`String!`](scalars.md#string) |  |  |
| `min_length` | [`Int`](scalars.md#int) |  | `1` |

## callResolveCoreference

> Coreference resolution

**Type:** [`CorefResult`](objects.md#corefresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String!`](scalars.md#string) | Text to perform coreference resolution on |  |

## callSentimentAnalysis

> Sentiment analisys

**Type:** [`[SentimentAnalysisResult]`](objects.md#sentimentanalysisresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `input` | [`String!`](scalars.md#string) | Text to perform sentiment analysis on |  |

## callShowDocs

**Type:** [`ServiceInfo`](objects.md#serviceinfo)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `service` | [`ServiceName`](enums.md#servicename) |  |  |

## callSpeechToText

> Convert speech to text

**Type:** [`[STTResult]`](objects.md#sttresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `audioB64` | [`String!`](scalars.md#string) |  |  |
| `config` | [`STTConfig`](inputs.md#sttconfig) |  |  |

## callTextToSpeech

> Convert text to speech

**Type:** [`TTSResult`](objects.md#ttsresult)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `config` | [`TTSConfig`](inputs.md#ttsconfig) |  |  |
| `text` | [`String!`](scalars.md#string) |  |  |

## conceptnet_data

> fetch data from the table: "conceptnet.data"

**Type:** [`[conceptnet_data!]!`](objects.md#conceptnet_data)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[conceptnet_data_select_column!]`](enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet_data_aggregate

> fetch aggregated fields from the table: "conceptnet.data"

**Type:** [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[conceptnet_data_select_column!]`](enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet_search_relations

> execute function "conceptnet.search_relations" which returns "conceptnet.data"

**Type:** [`[conceptnet_data!]!`](objects.md#conceptnet_data)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `args` | [`conceptnet_search_relations_args!`](inputs.md#conceptnet_search_relations_args) | input parameters for function "conceptnet.search_relations" |  |
| `distinct_on` | [`[conceptnet_data_select_column!]`](enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet_search_relations_aggregate

> execute function "conceptnet.search_relations" and query aggregates on result of table type "conceptnet.data"

**Type:** [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `args` | [`conceptnet_search_relations_args!`](inputs.md#conceptnet_search_relations_args) | input parameters for function "conceptnet.search_relations" |  |
| `distinct_on` | [`[conceptnet_data_select_column!]`](enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conversations

> An array relationship

**Type:** [`[conversations!]!`](objects.md#conversations)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[conversations_select_column!]`](enums.md#conversations_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[conversations_order_by!]`](inputs.md#conversations_order_by) | sort the rows by one or more columns |  |
| `where` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) | filter the rows returned |  |

## deprecatedCallNlpDoc

> Document processing

**Type:** [`NlpDoc`](objects.md#nlpdoc)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `disable` | [`[String]`](scalars.md#string) | List of pipes to disable | `[]` |
| `input` | [`String!`](scalars.md#string) | Text to perform process |  |
| `model` | [`String`](scalars.md#string) | Name of the spaCy model to use | `"en_core_web_md"` |

## developers

> fetch data from the table: "developers"

**Type:** [`[developers!]!`](objects.md#developers)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[developers_select_column!]`](enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[developers_order_by!]`](inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](inputs.md#developers_bool_exp) | filter the rows returned |  |

## developers_aggregate

> fetch aggregated fields from the table: "developers"

**Type:** [`developers_aggregate!`](objects.md#developers_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[developers_select_column!]`](enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[developers_order_by!]`](inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](inputs.md#developers_bool_exp) | filter the rows returned |  |

## events

> An array relationship

**Type:** [`[events!]!`](objects.md#events)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[events_select_column!]`](enums.md#events_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[events_order_by!]`](inputs.md#events_order_by) | sort the rows by one or more columns |  |
| `where` | [`events_bool_exp`](inputs.md#events_bool_exp) | filter the rows returned |  |

## events_aggregate

> An aggregate relationship

**Type:** [`events_aggregate!`](objects.md#events_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[events_select_column!]`](enums.md#events_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[events_order_by!]`](inputs.md#events_order_by) | sort the rows by one or more columns |  |
| `where` | [`events_bool_exp`](inputs.md#events_bool_exp) | filter the rows returned |  |

## history

> fetch data from the table: "history"

**Type:** [`[history!]!`](objects.md#history)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[history_select_column!]`](enums.md#history_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[history_order_by!]`](inputs.md#history_order_by) | sort the rows by one or more columns |  |
| `where` | [`history_bool_exp`](inputs.md#history_bool_exp) | filter the rows returned |  |

## kv_store

> An array relationship

**Type:** [`[kv_store!]!`](objects.md#kv_store)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[kv_store_select_column!]`](enums.md#kv_store_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[kv_store_order_by!]`](inputs.md#kv_store_order_by) | sort the rows by one or more columns |  |
| `where` | [`kv_store_bool_exp`](inputs.md#kv_store_bool_exp) | filter the rows returned |  |

## kv_store_by_pk

> fetch data from the table: "kv_store" using primary key columns

**Type:** [`kv_store`](objects.md#kv_store)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `key` | [`String!`](scalars.md#string) |  |  |
| `scope` | [`String!`](scalars.md#string) |  |  |
| `scope_object_id` | [`Int!`](scalars.md#int) |  |  |

## last_utterance

> fetch data from the table: "last_utterance"

**Type:** [`[last_utterance!]!`](objects.md#last_utterance)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[last_utterance_select_column!]`](enums.md#last_utterance_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[last_utterance_order_by!]`](inputs.md#last_utterance_order_by) | sort the rows by one or more columns |  |
| `where` | [`last_utterance_bool_exp`](inputs.md#last_utterance_bool_exp) | filter the rows returned |  |

## me

> execute function "me" which returns "developers"

**Type:** [`[developers!]!`](objects.md#developers)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[developers_select_column!]`](enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[developers_order_by!]`](inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](inputs.md#developers_bool_exp) | filter the rows returned |  |

## me_aggregate

> execute function "me" and query aggregates on result of table type "developers"

**Type:** [`developers_aggregate!`](objects.md#developers_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[developers_select_column!]`](enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[developers_order_by!]`](inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](inputs.md#developers_bool_exp) | filter the rows returned |  |

## utterances

> An array relationship

**Type:** [`[utterances!]!`](objects.md#utterances)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `distinct_on` | [`[utterances_select_column!]`](enums.md#utterances_select_column) | distinct select on columns |  |
| `limit` | [`Int`](scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](scalars.md#int) | skip the first n rows. Use only with order_by |  |
| `order_by` | [`[utterances_order_by!]`](inputs.md#utterances_order_by) | sort the rows by one or more columns |  |
| `where` | [`utterances_bool_exp`](inputs.md#utterances_bool_exp) | filter the rows returned |  |


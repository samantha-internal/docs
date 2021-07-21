# Enums

## <a name="aceoutputtype"></a>ACEOutputType

> Output format

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `drs` |  | no |
| `drshtml` |  | no |
| `drspp` |  | no |
| `drsxml` |  | no |
| `fol` |  | no |
| `owlfss` |  | no |
| `owlfsspp` |  | no |
| `owlrdf` |  | no |
| `owlxml` |  | no |
| `paraphrase` |  | no |
| `paraphrase1` |  | no |
| `paraphrase2` |  | no |
| `pnf` |  | no |
| `ruleml` |  | no |
| `syntax` |  | no |
| `syntaxd` |  | no |
| `syntaxdpp` |  | no |
| `syntaxpp` |  | no |
| `tokens` |  | no |
| `tptp` |  | no |

## <a name="agent"></a>Agent

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `BOT` |  | no |
| `USER` |  | no |

## <a name="audioencoding"></a>AudioEncoding

> Audio encoding

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `AUDIO_ENCODING_UNSPECIFIED` |  | no |
| `LINEAR16` |  | no |
| `MP3` |  | no |
| `OGG_OPUS` |  | no |

## <a name="category"></a>Category

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `oEffect` |  | no |
| `oReact` |  | no |
| `oWant` |  | no |
| `xAttr` |  | no |
| `xEffect` |  | no |
| `xIntent` |  | no |
| `xNeed` |  | no |
| `xReact` |  | no |
| `xWant` |  | no |

## <a name="encoding"></a>Encoding

> Audio encoding

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `AMR` |  | no |
| `AMR_WB` |  | no |
| `ENCODING_UNSPECIFIED` |  | no |
| `FLAC` |  | no |
| `LINEAR16` |  | no |
| `MP3` |  | no |
| `MULAW` |  | no |
| `OGG_OPUS` |  | no |
| `SPEEX_WITH_HEADER_BYTE` |  | no |

## <a name="relation"></a>Relation

> Relation type

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `AtLocation` |  | no |
| `CapableOf` |  | no |
| `Causes` |  | no |
| `CausesDesire` |  | no |
| `CreatedBy` |  | no |
| `DefinedAs` |  | no |
| `DesireOf` |  | no |
| `Desires` |  | no |
| `HasA` |  | no |
| `HasFirstSubevent` |  | no |
| `HasLastSubevent` |  | no |
| `HasPainCharacter` |  | no |
| `HasPainIntensity` |  | no |
| `HasPrerequisite` |  | no |
| `HasProperty` |  | no |
| `HasSubevent` |  | no |
| `InheritsFrom` |  | no |
| `InstanceOf` |  | no |
| `IsA` |  | no |
| `LocatedNear` |  | no |
| `LocationOfAction` |  | no |
| `MadeOf` |  | no |
| `MotivatedByGoal` |  | no |
| `NotCapableOf` |  | no |
| `NotDesires` |  | no |
| `NotHasA` |  | no |
| `NotHasProperty` |  | no |
| `NotIsA` |  | no |
| `NotMadeOf` |  | no |
| `PartOf` |  | no |
| `ReceivesAction` |  | no |
| `RelatedTo` |  | no |
| `SymbolOf` |  | no |
| `UsedFor` |  | no |

## <a name="servicename"></a>ServiceName

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `ace_parser` |  | no |
| `chitchat_service` |  | no |
| `commonsense` |  | no |
| `compose_services` |  | no |
| `context_frame_parser` |  | no |
| `docs` |  | no |
| `faq_service` |  | no |
| `intent_matcher` |  | no |
| `nlu_service` |  | no |
| `paraphrase_sentences` |  | no |
| `sentence_similarity` |  | no |
| `speech_to_text` |  | no |
| `text_to_speech` |  | no |
| `topic_classification` |  | no |
| `turn_prediction` |  | no |
| `voice_css_render` |  | no |

## <a name="__typekind"></a>__TypeKind

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `ENUM` |  | no |
| `INPUT_OBJECT` |  | no |
| `INTERFACE` |  | no |
| `LIST` |  | no |
| `NON_NULL` |  | no |
| `OBJECT` |  | no |
| `SCALAR` |  | no |
| `UNION` |  | no |

## <a name="apps_constraint"></a>apps_constraint

> unique or primary key constraints on table "apps"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `apps_object_id_key` | unique or primary key constraint | no |
| `apps_slug_key` | unique or primary key constraint | no |

## <a name="apps_select_column"></a>apps_select_column

> select columns of table "apps"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `created_at` | column name | no |
| `developer_id` | column name | no |
| `metadata` | column name | no |
| `object_id` | column name | no |
| `scope_name` | column name | no |
| `slug` | column name | no |
| `status` | column name | no |

## <a name="apps_update_column"></a>apps_update_column

> update columns of table "apps"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `scope_name` | column name | no |
| `slug` | column name | no |
| `status` | column name | no |

## <a name="atomic_data_select_column"></a>atomic_data_select_column

> select columns of table "atomic.data"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `event` | column name | no |
| `o_effect` | column name | no |
| `o_react` | column name | no |
| `o_want` | column name | no |
| `prefix` | column name | no |
| `x_attr` | column name | no |
| `x_effect` | column name | no |
| `x_intent` | column name | no |
| `x_need` | column name | no |
| `x_react` | column name | no |
| `x_want` | column name | no |

## <a name="conceptnet_data_select_column"></a>conceptnet_data_select_column

> select columns of table "conceptnet.data"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `end` | column name | no |
| `relation` | column name | no |
| `start` | column name | no |
| `uri` | column name | no |
| `weight` | column name | no |

## <a name="conversations_constraint"></a>conversations_constraint

> unique or primary key constraints on table "conversations"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `conversations_object_id_key` | unique or primary key constraint | no |

## <a name="conversations_select_column"></a>conversations_select_column

> select columns of table "conversations"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `app_id` | column name | no |
| `created_at` | column name | no |
| `destroyed_at` | column name | no |
| `end_user_id` | column name | no |
| `metadata` | column name | no |
| `object_id` | column name | no |
| `scope_name` | column name | no |

## <a name="conversations_update_column"></a>conversations_update_column

> update columns of table "conversations"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `scope_name` | column name | no |

## <a name="developers_select_column"></a>developers_select_column

> select columns of table "developers"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `active` | column name | no |
| `api_key` | column name | no |
| `created_at` | column name | no |
| `email` | column name | no |
| `github_handle` | column name | no |
| `metadata` | column name | no |
| `name` | column name | no |
| `object_id` | column name | no |
| `onboarded` | column name | no |
| `uid` | column name | no |

## <a name="events_select_column"></a>events_select_column

> select columns of table "events"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `action` | column name | no |
| `changed_fields` | column name | no |
| `developer_id` | column name | no |
| `table` | column name | no |
| `timestamp` | column name | no |

## <a name="history_select_column"></a>history_select_column

> select columns of table "history"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `conversation_id` | column name | no |
| `interval` | column name | no |
| `updated_at` | column name | no |
| `utterances` | column name | no |
| `window` | column name | no |

## <a name="kv_store_select_column"></a>kv_store_select_column

> select columns of table "kv_store"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `created_at` | column name | no |
| `created_by` | column name | no |
| `key` | column name | no |
| `metadata` | column name | no |
| `object_id` | column name | no |
| `scope` | column name | no |
| `scope_object_id` | column name | no |
| `updated_at` | column name | no |
| `value` | column name | no |

## <a name="last_utterance_select_column"></a>last_utterance_select_column

> select columns of table "last_utterance"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `conversation_id` | column name | no |
| `interval` | column name | no |
| `speaker_type` | column name | no |
| `updated_at` | column name | no |
| `utterance` | column name | no |

## <a name="order_by"></a>order_by

> column ordering options

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `asc` | in ascending order, nulls last | no |
| `asc_nulls_first` | in ascending order, nulls first | no |
| `asc_nulls_last` | in ascending order, nulls last | no |
| `desc` | in descending order, nulls first | no |
| `desc_nulls_first` | in descending order, nulls first | no |
| `desc_nulls_last` | in descending order, nulls last | no |

## <a name="speaker_type_enum_enum"></a>speaker_type_enum_enum

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `bot` |  | no |
| `user` |  | no |

## <a name="utterances_select_column"></a>utterances_select_column

> select columns of table "utterances"

### Values

| Name | Description | Deprecated |
| --- | --- | --- |
| `conversation_id` | column name | no |
| `end_user_id` | column name | no |
| `normalized_utterance` | column name | no |
| `speaker_type` | column name | no |
| `timestamp` | column name | no |
| `utterance` | column name | no |


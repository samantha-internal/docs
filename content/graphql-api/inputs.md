# Inputs

## <a name="boolean_comparison_exp"></a>Boolean_comparison_exp

> Boolean expression to compare columns of type "Boolean". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`Boolean`](scalars.md#boolean) |  |  |
| `_gt` | [`Boolean`](scalars.md#boolean) |  |  |
| `_gte` | [`Boolean`](scalars.md#boolean) |  |  |
| `_in` | [`[Boolean!]`](scalars.md#boolean) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lte` | [`Boolean`](scalars.md#boolean) |  |  |
| `_neq` | [`Boolean`](scalars.md#boolean) |  |  |
| `_nin` | [`[Boolean!]`](scalars.md#boolean) |  |  |

## <a name="contextobject"></a>ContextObject

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `content` | [`String`](scalars.md#string) | Dialog turn content |  |

## <a name="inputpipe"></a>InputPipe

> Pipe input type

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `context` | [`JSON`](scalars.md#json) | Variable bindings |  |
| `op` | [`String`](scalars.md#string) | Service query name |  |
| `transform` | [`String`](scalars.md#string) | Transform logic |  |

## <a name="int_comparison_exp"></a>Int_comparison_exp

> Boolean expression to compare columns of type "Int". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`Int`](scalars.md#int) |  |  |
| `_gt` | [`Int`](scalars.md#int) |  |  |
| `_gte` | [`Int`](scalars.md#int) |  |  |
| `_in` | [`[Int!]`](scalars.md#int) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`Int`](scalars.md#int) |  |  |
| `_lte` | [`Int`](scalars.md#int) |  |  |
| `_neq` | [`Int`](scalars.md#int) |  |  |
| `_nin` | [`[Int!]`](scalars.md#int) |  |  |

## <a name="sttconfig"></a>STTConfig

> Speech to text config

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `encoding` | [`Encoding`](enums.md#encoding) | Audio encoding |  |
| `languageCode` | [`String`](scalars.md#string) | Language code |  |
| `maxAlternatives` | [`Int`](scalars.md#int) | Maximum number of the output alternatives |  |
| `profanityFilter` | [`Boolean`](scalars.md#boolean) | Profanity filter flag |  |
| `sampleRate` | [`Int`](scalars.md#int) | Audio Sample rate |  |

## <a name="string_comparison_exp"></a>String_comparison_exp

> Boolean expression to compare columns of type "String". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`String`](scalars.md#string) |  |  |
| `_gt` | [`String`](scalars.md#string) |  |  |
| `_gte` | [`String`](scalars.md#string) |  |  |
| `_ilike` | [`String`](scalars.md#string) | does the column match the given case-insensitive pattern |  |
| `_in` | [`[String!]`](scalars.md#string) |  |  |
| `_iregex` | [`String`](scalars.md#string) | does the column match the given POSIX regular expression, case insensitive |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_like` | [`String`](scalars.md#string) | does the column match the given pattern |  |
| `_lt` | [`String`](scalars.md#string) |  |  |
| `_lte` | [`String`](scalars.md#string) |  |  |
| `_neq` | [`String`](scalars.md#string) |  |  |
| `_nilike` | [`String`](scalars.md#string) | does the column NOT match the given case-insensitive pattern |  |
| `_nin` | [`[String!]`](scalars.md#string) |  |  |
| `_niregex` | [`String`](scalars.md#string) | does the column NOT match the given POSIX regular expression, case insensitive |  |
| `_nlike` | [`String`](scalars.md#string) | does the column NOT match the given pattern |  |
| `_nregex` | [`String`](scalars.md#string) | does the column NOT match the given POSIX regular expression, case sensitive |  |
| `_nsimilar` | [`String`](scalars.md#string) | does the column NOT match the given SQL regular expression |  |
| `_regex` | [`String`](scalars.md#string) | does the column match the given POSIX regular expression, case sensitive |  |
| `_similar` | [`String`](scalars.md#string) | does the column match the given SQL regular expression |  |

## <a name="ttsconfig"></a>TTSConfig

> Input config

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `encoding` | [`AudioEncoding`](enums.md#audioencoding) | Audio encoding |  |
| `languageCode` | [`String`](scalars.md#string) | Language code |  |
| `sampleRate` | [`Float`](scalars.md#float) | Audio sample rate |  |
| `voiceGender` | [`String`](scalars.md#string) | Voice gender |  |

## <a name="turn"></a>Turn

> An object representing a single turn by an agent

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `agent` | [`Agent`](enums.md#agent) |  |  |
| `said` | [`String`](scalars.md#string) |  |  |

## <a name="_text_comparison_exp"></a>_text_comparison_exp

> Boolean expression to compare columns of type "_text". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`_text`](scalars.md#_text) |  |  |
| `_gt` | [`_text`](scalars.md#_text) |  |  |
| `_gte` | [`_text`](scalars.md#_text) |  |  |
| `_in` | [`[_text!]`](scalars.md#_text) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`_text`](scalars.md#_text) |  |  |
| `_lte` | [`_text`](scalars.md#_text) |  |  |
| `_neq` | [`_text`](scalars.md#_text) |  |  |
| `_nin` | [`[_text!]`](scalars.md#_text) |  |  |

## <a name="app_status_comparison_exp"></a>app_status_comparison_exp

> Boolean expression to compare columns of type "app_status". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`app_status`](scalars.md#app_status) |  |  |
| `_gt` | [`app_status`](scalars.md#app_status) |  |  |
| `_gte` | [`app_status`](scalars.md#app_status) |  |  |
| `_in` | [`[app_status!]`](scalars.md#app_status) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`app_status`](scalars.md#app_status) |  |  |
| `_lte` | [`app_status`](scalars.md#app_status) |  |  |
| `_neq` | [`app_status`](scalars.md#app_status) |  |  |
| `_nin` | [`[app_status!]`](scalars.md#app_status) |  |  |

## <a name="apps_aggregate_order_by"></a>apps_aggregate_order_by

> order by aggregate values of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `avg` | [`apps_avg_order_by`](inputs.md#apps_avg_order_by) |  |  |
| `count` | [`order_by`](enums.md#order_by) |  |  |
| `max` | [`apps_max_order_by`](inputs.md#apps_max_order_by) |  |  |
| `min` | [`apps_min_order_by`](inputs.md#apps_min_order_by) |  |  |
| `stddev` | [`apps_stddev_order_by`](inputs.md#apps_stddev_order_by) |  |  |
| `stddev_pop` | [`apps_stddev_pop_order_by`](inputs.md#apps_stddev_pop_order_by) |  |  |
| `stddev_samp` | [`apps_stddev_samp_order_by`](inputs.md#apps_stddev_samp_order_by) |  |  |
| `sum` | [`apps_sum_order_by`](inputs.md#apps_sum_order_by) |  |  |
| `var_pop` | [`apps_var_pop_order_by`](inputs.md#apps_var_pop_order_by) |  |  |
| `var_samp` | [`apps_var_samp_order_by`](inputs.md#apps_var_samp_order_by) |  |  |
| `variance` | [`apps_variance_order_by`](inputs.md#apps_variance_order_by) |  |  |

## <a name="apps_avg_order_by"></a>apps_avg_order_by

> order by avg() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_bool_exp"></a>apps_bool_exp

> Boolean expression to filter rows from the table "apps". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[apps_bool_exp!]`](inputs.md#apps_bool_exp) |  |  |
| `_not` | [`apps_bool_exp`](inputs.md#apps_bool_exp) |  |  |
| `_or` | [`[apps_bool_exp!]`](inputs.md#apps_bool_exp) |  |  |
| `conversations` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |
| `created_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `developer` | [`developers_bool_exp`](inputs.md#developers_bool_exp) |  |  |
| `developer_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `kv_store` | [`kv_store_bool_exp`](inputs.md#kv_store_bool_exp) |  |  |
| `metadata` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `object_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `scope_name` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `slug` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `status` | [`app_status_comparison_exp`](inputs.md#app_status_comparison_exp) |  |  |

## <a name="apps_insert_input"></a>apps_insert_input

> input type for inserting data into table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversations` | [`conversations_arr_rel_insert_input`](inputs.md#conversations_arr_rel_insert_input) |  |  |
| `scope_name` | [`String`](scalars.md#string) |  |  |
| `slug` | [`String`](scalars.md#string) |  |  |
| `status` | [`app_status`](scalars.md#app_status) |  |  |

## <a name="apps_max_order_by"></a>apps_max_order_by

> order by max() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |
| `slug` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_min_order_by"></a>apps_min_order_by

> order by min() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |
| `slug` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_obj_rel_insert_input"></a>apps_obj_rel_insert_input

> input type for inserting object relation for remote table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `data` | [`apps_insert_input!`](inputs.md#apps_insert_input) |  |  |
| `on_conflict` | [`apps_on_conflict`](inputs.md#apps_on_conflict) | on conflict condition |  |

## <a name="apps_on_conflict"></a>apps_on_conflict

> on conflict condition type for table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `constraint` | [`apps_constraint!`](enums.md#apps_constraint) |  |  |
| `update_columns` | [`[apps_update_column!]!`](enums.md#apps_update_column) |  |  |
| `where` | [`apps_bool_exp`](inputs.md#apps_bool_exp) |  |  |

## <a name="apps_order_by"></a>apps_order_by

> Ordering options when selecting data from "apps".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversations_aggregate` | [`conversations_aggregate_order_by`](inputs.md#conversations_aggregate_order_by) |  |  |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `developer` | [`developers_order_by`](inputs.md#developers_order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `kv_store_aggregate` | [`kv_store_aggregate_order_by`](inputs.md#kv_store_aggregate_order_by) |  |  |
| `metadata` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |
| `slug` | [`order_by`](enums.md#order_by) |  |  |
| `status` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_set_input"></a>apps_set_input

> input type for updating data in table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `scope_name` | [`String`](scalars.md#string) |  |  |
| `slug` | [`String`](scalars.md#string) |  |  |
| `status` | [`app_status`](scalars.md#app_status) |  |  |

## <a name="apps_stddev_order_by"></a>apps_stddev_order_by

> order by stddev() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_stddev_pop_order_by"></a>apps_stddev_pop_order_by

> order by stddev_pop() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_stddev_samp_order_by"></a>apps_stddev_samp_order_by

> order by stddev_samp() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_sum_order_by"></a>apps_sum_order_by

> order by sum() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_var_pop_order_by"></a>apps_var_pop_order_by

> order by var_pop() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_var_samp_order_by"></a>apps_var_samp_order_by

> order by var_samp() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="apps_variance_order_by"></a>apps_variance_order_by

> order by variance() on columns of table "apps"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="atomic_data_bool_exp"></a>atomic_data_bool_exp

> Boolean expression to filter rows from the table "atomic.data". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[atomic_data_bool_exp!]`](inputs.md#atomic_data_bool_exp) |  |  |
| `_not` | [`atomic_data_bool_exp`](inputs.md#atomic_data_bool_exp) |  |  |
| `_or` | [`[atomic_data_bool_exp!]`](inputs.md#atomic_data_bool_exp) |  |  |
| `event` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `o_effect` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `o_react` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `o_want` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `prefix` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_attr` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_effect` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_intent` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_need` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_react` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |
| `x_want` | [`_text_comparison_exp`](inputs.md#_text_comparison_exp) |  |  |

## <a name="atomic_data_order_by"></a>atomic_data_order_by

> Ordering options when selecting data from "atomic.data".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `event` | [`order_by`](enums.md#order_by) |  |  |
| `o_effect` | [`order_by`](enums.md#order_by) |  |  |
| `o_react` | [`order_by`](enums.md#order_by) |  |  |
| `o_want` | [`order_by`](enums.md#order_by) |  |  |
| `prefix` | [`order_by`](enums.md#order_by) |  |  |
| `x_attr` | [`order_by`](enums.md#order_by) |  |  |
| `x_effect` | [`order_by`](enums.md#order_by) |  |  |
| `x_intent` | [`order_by`](enums.md#order_by) |  |  |
| `x_need` | [`order_by`](enums.md#order_by) |  |  |
| `x_react` | [`order_by`](enums.md#order_by) |  |  |
| `x_want` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conceptnet_data_bool_exp"></a>conceptnet_data_bool_exp

> Boolean expression to filter rows from the table "conceptnet.data". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[conceptnet_data_bool_exp!]`](inputs.md#conceptnet_data_bool_exp) |  |  |
| `_not` | [`conceptnet_data_bool_exp`](inputs.md#conceptnet_data_bool_exp) |  |  |
| `_or` | [`[conceptnet_data_bool_exp!]`](inputs.md#conceptnet_data_bool_exp) |  |  |
| `end` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `relation` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `start` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `uri` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `weight` | [`numeric_comparison_exp`](inputs.md#numeric_comparison_exp) |  |  |

## <a name="conceptnet_data_order_by"></a>conceptnet_data_order_by

> Ordering options when selecting data from "conceptnet.data".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `end` | [`order_by`](enums.md#order_by) |  |  |
| `relation` | [`order_by`](enums.md#order_by) |  |  |
| `start` | [`order_by`](enums.md#order_by) |  |  |
| `uri` | [`order_by`](enums.md#order_by) |  |  |
| `weight` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conceptnet_search_relations_args"></a>conceptnet_search_relations_args

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `limit_to` | [`numeric`](scalars.md#numeric) |  |  |
| `search` | [`String`](scalars.md#string) |  |  |

## <a name="conversations_aggregate_order_by"></a>conversations_aggregate_order_by

> order by aggregate values of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `avg` | [`conversations_avg_order_by`](inputs.md#conversations_avg_order_by) |  |  |
| `count` | [`order_by`](enums.md#order_by) |  |  |
| `max` | [`conversations_max_order_by`](inputs.md#conversations_max_order_by) |  |  |
| `min` | [`conversations_min_order_by`](inputs.md#conversations_min_order_by) |  |  |
| `stddev` | [`conversations_stddev_order_by`](inputs.md#conversations_stddev_order_by) |  |  |
| `stddev_pop` | [`conversations_stddev_pop_order_by`](inputs.md#conversations_stddev_pop_order_by) |  |  |
| `stddev_samp` | [`conversations_stddev_samp_order_by`](inputs.md#conversations_stddev_samp_order_by) |  |  |
| `sum` | [`conversations_sum_order_by`](inputs.md#conversations_sum_order_by) |  |  |
| `var_pop` | [`conversations_var_pop_order_by`](inputs.md#conversations_var_pop_order_by) |  |  |
| `var_samp` | [`conversations_var_samp_order_by`](inputs.md#conversations_var_samp_order_by) |  |  |
| `variance` | [`conversations_variance_order_by`](inputs.md#conversations_variance_order_by) |  |  |

## <a name="conversations_arr_rel_insert_input"></a>conversations_arr_rel_insert_input

> input type for inserting array relation for remote table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `data` | [`[conversations_insert_input!]!`](inputs.md#conversations_insert_input) |  |  |
| `on_conflict` | [`conversations_on_conflict`](inputs.md#conversations_on_conflict) | on conflict condition |  |

## <a name="conversations_avg_order_by"></a>conversations_avg_order_by

> order by avg() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_bool_exp"></a>conversations_bool_exp

> Boolean expression to filter rows from the table "conversations". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[conversations_bool_exp!]`](inputs.md#conversations_bool_exp) |  |  |
| `_not` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |
| `_or` | [`[conversations_bool_exp!]`](inputs.md#conversations_bool_exp) |  |  |
| `app` | [`apps_bool_exp`](inputs.md#apps_bool_exp) |  |  |
| `app_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `created_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `destroyed_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `end_user_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `kv_store` | [`kv_store_bool_exp`](inputs.md#kv_store_bool_exp) |  |  |
| `metadata` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `object_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `scope_name` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `utterances` | [`utterances_bool_exp`](inputs.md#utterances_bool_exp) |  |  |

## <a name="conversations_insert_input"></a>conversations_insert_input

> input type for inserting data into table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app` | [`apps_obj_rel_insert_input`](inputs.md#apps_obj_rel_insert_input) |  |  |
| `app_id` | [`Int`](scalars.md#int) |  |  |
| `end_user_id` | [`Int`](scalars.md#int) |  |  |
| `scope_name` | [`String`](scalars.md#string) |  |  |
| `utterances` | [`utterances_arr_rel_insert_input`](inputs.md#utterances_arr_rel_insert_input) |  |  |

## <a name="conversations_max_order_by"></a>conversations_max_order_by

> order by max() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `destroyed_at` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_min_order_by"></a>conversations_min_order_by

> order by min() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `destroyed_at` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_obj_rel_insert_input"></a>conversations_obj_rel_insert_input

> input type for inserting object relation for remote table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `data` | [`conversations_insert_input!`](inputs.md#conversations_insert_input) |  |  |
| `on_conflict` | [`conversations_on_conflict`](inputs.md#conversations_on_conflict) | on conflict condition |  |

## <a name="conversations_on_conflict"></a>conversations_on_conflict

> on conflict condition type for table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `constraint` | [`conversations_constraint!`](enums.md#conversations_constraint) |  |  |
| `update_columns` | [`[conversations_update_column!]!`](enums.md#conversations_update_column) |  |  |
| `where` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |

## <a name="conversations_order_by"></a>conversations_order_by

> Ordering options when selecting data from "conversations".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app` | [`apps_order_by`](inputs.md#apps_order_by) |  |  |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `destroyed_at` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `kv_store_aggregate` | [`kv_store_aggregate_order_by`](inputs.md#kv_store_aggregate_order_by) |  |  |
| `metadata` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_name` | [`order_by`](enums.md#order_by) |  |  |
| `utterances_aggregate` | [`utterances_aggregate_order_by`](inputs.md#utterances_aggregate_order_by) |  |  |

## <a name="conversations_set_input"></a>conversations_set_input

> input type for updating data in table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `scope_name` | [`String`](scalars.md#string) |  |  |

## <a name="conversations_stddev_order_by"></a>conversations_stddev_order_by

> order by stddev() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_stddev_pop_order_by"></a>conversations_stddev_pop_order_by

> order by stddev_pop() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_stddev_samp_order_by"></a>conversations_stddev_samp_order_by

> order by stddev_samp() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_sum_order_by"></a>conversations_sum_order_by

> order by sum() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_var_pop_order_by"></a>conversations_var_pop_order_by

> order by var_pop() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_var_samp_order_by"></a>conversations_var_samp_order_by

> order by var_samp() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="conversations_variance_order_by"></a>conversations_variance_order_by

> order by variance() on columns of table "conversations"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `app_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="developers_bool_exp"></a>developers_bool_exp

> Boolean expression to filter rows from the table "developers". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[developers_bool_exp!]`](inputs.md#developers_bool_exp) |  |  |
| `_not` | [`developers_bool_exp`](inputs.md#developers_bool_exp) |  |  |
| `_or` | [`[developers_bool_exp!]`](inputs.md#developers_bool_exp) |  |  |
| `active` | [`Boolean_comparison_exp`](inputs.md#boolean_comparison_exp) |  |  |
| `api_key` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `apps` | [`apps_bool_exp`](inputs.md#apps_bool_exp) |  |  |
| `created_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `email` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `events` | [`events_bool_exp`](inputs.md#events_bool_exp) |  |  |
| `github_handle` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `kv_stores` | [`kv_store_bool_exp`](inputs.md#kv_store_bool_exp) |  |  |
| `metadata` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `name` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `object_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `onboarded` | [`Boolean_comparison_exp`](inputs.md#boolean_comparison_exp) |  |  |
| `uid` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |

## <a name="developers_order_by"></a>developers_order_by

> Ordering options when selecting data from "developers".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `active` | [`order_by`](enums.md#order_by) |  |  |
| `api_key` | [`order_by`](enums.md#order_by) |  |  |
| `apps_aggregate` | [`apps_aggregate_order_by`](inputs.md#apps_aggregate_order_by) |  |  |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `email` | [`order_by`](enums.md#order_by) |  |  |
| `events_aggregate` | [`events_aggregate_order_by`](inputs.md#events_aggregate_order_by) |  |  |
| `github_handle` | [`order_by`](enums.md#order_by) |  |  |
| `kv_stores_aggregate` | [`kv_store_aggregate_order_by`](inputs.md#kv_store_aggregate_order_by) |  |  |
| `metadata` | [`order_by`](enums.md#order_by) |  |  |
| `name` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `onboarded` | [`order_by`](enums.md#order_by) |  |  |
| `uid` | [`order_by`](enums.md#order_by) |  |  |

## <a name="developers_set_input"></a>developers_set_input

> input type for updating data in table "developers"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `email` | [`String`](scalars.md#string) |  |  |
| `github_handle` | [`String`](scalars.md#string) |  |  |
| `name` | [`String`](scalars.md#string) |  |  |

## <a name="events_aggregate_order_by"></a>events_aggregate_order_by

> order by aggregate values of table "events"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `count` | [`order_by`](enums.md#order_by) |  |  |
| `max` | [`events_max_order_by`](inputs.md#events_max_order_by) |  |  |
| `min` | [`events_min_order_by`](inputs.md#events_min_order_by) |  |  |

## <a name="events_bool_exp"></a>events_bool_exp

> Boolean expression to filter rows from the table "events". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[events_bool_exp!]`](inputs.md#events_bool_exp) |  |  |
| `_not` | [`events_bool_exp`](inputs.md#events_bool_exp) |  |  |
| `_or` | [`[events_bool_exp!]`](inputs.md#events_bool_exp) |  |  |
| `action` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `changed_fields` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `developer_id` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `table` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `timestamp` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |

## <a name="events_max_order_by"></a>events_max_order_by

> order by max() on columns of table "events"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `action` | [`order_by`](enums.md#order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `table` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |

## <a name="events_min_order_by"></a>events_min_order_by

> order by min() on columns of table "events"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `action` | [`order_by`](enums.md#order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `table` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |

## <a name="events_order_by"></a>events_order_by

> Ordering options when selecting data from "events".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `action` | [`order_by`](enums.md#order_by) |  |  |
| `changed_fields` | [`order_by`](enums.md#order_by) |  |  |
| `developer_id` | [`order_by`](enums.md#order_by) |  |  |
| `table` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |

## <a name="history_bool_exp"></a>history_bool_exp

> Boolean expression to filter rows from the table "history". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[history_bool_exp!]`](inputs.md#history_bool_exp) |  |  |
| `_not` | [`history_bool_exp`](inputs.md#history_bool_exp) |  |  |
| `_or` | [`[history_bool_exp!]`](inputs.md#history_bool_exp) |  |  |
| `conversation` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |
| `conversation_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `interval` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `updated_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `utterances` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `window` | [`tstzrange_comparison_exp`](inputs.md#tstzrange_comparison_exp) |  |  |

## <a name="history_order_by"></a>history_order_by

> Ordering options when selecting data from "history".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation` | [`conversations_order_by`](inputs.md#conversations_order_by) |  |  |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `interval` | [`order_by`](enums.md#order_by) |  |  |
| `updated_at` | [`order_by`](enums.md#order_by) |  |  |
| `utterances` | [`order_by`](enums.md#order_by) |  |  |
| `window` | [`order_by`](enums.md#order_by) |  |  |

## <a name="jsonb_comparison_exp"></a>jsonb_comparison_exp

> Boolean expression to compare columns of type "jsonb". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_contained_in` | [`jsonb`](scalars.md#jsonb) | is the column contained in the given json value |  |
| `_contains` | [`jsonb`](scalars.md#jsonb) | does the column contain the given json value at the top level |  |
| `_eq` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_gt` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_gte` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_has_key` | [`String`](scalars.md#string) | does the string exist as a top-level key in the column |  |
| `_has_keys_all` | [`[String!]`](scalars.md#string) | do all of these strings exist as top-level keys in the column |  |
| `_has_keys_any` | [`[String!]`](scalars.md#string) | do any of these strings exist as top-level keys in the column |  |
| `_in` | [`[jsonb!]`](scalars.md#jsonb) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_lte` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_neq` | [`jsonb`](scalars.md#jsonb) |  |  |
| `_nin` | [`[jsonb!]`](scalars.md#jsonb) |  |  |

## <a name="kv_store_aggregate_order_by"></a>kv_store_aggregate_order_by

> order by aggregate values of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `avg` | [`kv_store_avg_order_by`](inputs.md#kv_store_avg_order_by) |  |  |
| `count` | [`order_by`](enums.md#order_by) |  |  |
| `max` | [`kv_store_max_order_by`](inputs.md#kv_store_max_order_by) |  |  |
| `min` | [`kv_store_min_order_by`](inputs.md#kv_store_min_order_by) |  |  |
| `stddev` | [`kv_store_stddev_order_by`](inputs.md#kv_store_stddev_order_by) |  |  |
| `stddev_pop` | [`kv_store_stddev_pop_order_by`](inputs.md#kv_store_stddev_pop_order_by) |  |  |
| `stddev_samp` | [`kv_store_stddev_samp_order_by`](inputs.md#kv_store_stddev_samp_order_by) |  |  |
| `sum` | [`kv_store_sum_order_by`](inputs.md#kv_store_sum_order_by) |  |  |
| `var_pop` | [`kv_store_var_pop_order_by`](inputs.md#kv_store_var_pop_order_by) |  |  |
| `var_samp` | [`kv_store_var_samp_order_by`](inputs.md#kv_store_var_samp_order_by) |  |  |
| `variance` | [`kv_store_variance_order_by`](inputs.md#kv_store_variance_order_by) |  |  |

## <a name="kv_store_avg_order_by"></a>kv_store_avg_order_by

> order by avg() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_bool_exp"></a>kv_store_bool_exp

> Boolean expression to filter rows from the table "kv_store". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[kv_store_bool_exp!]`](inputs.md#kv_store_bool_exp) |  |  |
| `_not` | [`kv_store_bool_exp`](inputs.md#kv_store_bool_exp) |  |  |
| `_or` | [`[kv_store_bool_exp!]`](inputs.md#kv_store_bool_exp) |  |  |
| `created_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `created_by` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `developer` | [`developers_bool_exp`](inputs.md#developers_bool_exp) |  |  |
| `key` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `metadata` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |
| `object_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `scope` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `scope_object_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `updated_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `value` | [`jsonb_comparison_exp`](inputs.md#jsonb_comparison_exp) |  |  |

## <a name="kv_store_max_order_by"></a>kv_store_max_order_by

> order by max() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `key` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |
| `updated_at` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_min_order_by"></a>kv_store_min_order_by

> order by min() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `key` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |
| `updated_at` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_order_by"></a>kv_store_order_by

> Ordering options when selecting data from "kv_store".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_at` | [`order_by`](enums.md#order_by) |  |  |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `developer` | [`developers_order_by`](inputs.md#developers_order_by) |  |  |
| `key` | [`order_by`](enums.md#order_by) |  |  |
| `metadata` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |
| `updated_at` | [`order_by`](enums.md#order_by) |  |  |
| `value` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_stddev_order_by"></a>kv_store_stddev_order_by

> order by stddev() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_stddev_pop_order_by"></a>kv_store_stddev_pop_order_by

> order by stddev_pop() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_stddev_samp_order_by"></a>kv_store_stddev_samp_order_by

> order by stddev_samp() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_sum_order_by"></a>kv_store_sum_order_by

> order by sum() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_var_pop_order_by"></a>kv_store_var_pop_order_by

> order by var_pop() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_var_samp_order_by"></a>kv_store_var_samp_order_by

> order by var_samp() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="kv_store_variance_order_by"></a>kv_store_variance_order_by

> order by variance() on columns of table "kv_store"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `created_by` | [`order_by`](enums.md#order_by) |  |  |
| `object_id` | [`order_by`](enums.md#order_by) |  |  |
| `scope_object_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="last_utterance_bool_exp"></a>last_utterance_bool_exp

> Boolean expression to filter rows from the table "last_utterance". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[last_utterance_bool_exp!]`](inputs.md#last_utterance_bool_exp) |  |  |
| `_not` | [`last_utterance_bool_exp`](inputs.md#last_utterance_bool_exp) |  |  |
| `_or` | [`[last_utterance_bool_exp!]`](inputs.md#last_utterance_bool_exp) |  |  |
| `conversation` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |
| `conversation_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `interval` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `speaker_type` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `updated_at` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `utterance` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |

## <a name="last_utterance_order_by"></a>last_utterance_order_by

> Ordering options when selecting data from "last_utterance".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation` | [`conversations_order_by`](inputs.md#conversations_order_by) |  |  |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `interval` | [`order_by`](enums.md#order_by) |  |  |
| `speaker_type` | [`order_by`](enums.md#order_by) |  |  |
| `updated_at` | [`order_by`](enums.md#order_by) |  |  |
| `utterance` | [`order_by`](enums.md#order_by) |  |  |

## <a name="numeric_comparison_exp"></a>numeric_comparison_exp

> Boolean expression to compare columns of type "numeric". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`numeric`](scalars.md#numeric) |  |  |
| `_gt` | [`numeric`](scalars.md#numeric) |  |  |
| `_gte` | [`numeric`](scalars.md#numeric) |  |  |
| `_in` | [`[numeric!]`](scalars.md#numeric) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`numeric`](scalars.md#numeric) |  |  |
| `_lte` | [`numeric`](scalars.md#numeric) |  |  |
| `_neq` | [`numeric`](scalars.md#numeric) |  |  |
| `_nin` | [`[numeric!]`](scalars.md#numeric) |  |  |

## <a name="speaker_type_enum_enum_comparison_exp"></a>speaker_type_enum_enum_comparison_exp

> Boolean expression to compare columns of type "speaker_type_enum_enum". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`speaker_type_enum_enum`](enums.md#speaker_type_enum_enum) |  |  |
| `_in` | [`[speaker_type_enum_enum!]`](enums.md#speaker_type_enum_enum) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_neq` | [`speaker_type_enum_enum`](enums.md#speaker_type_enum_enum) |  |  |
| `_nin` | [`[speaker_type_enum_enum!]`](enums.md#speaker_type_enum_enum) |  |  |

## <a name="timestamptz_comparison_exp"></a>timestamptz_comparison_exp

> Boolean expression to compare columns of type "timestamptz". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_gt` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_gte` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_in` | [`[timestamptz!]`](scalars.md#timestamptz) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_lte` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_neq` | [`timestamptz`](scalars.md#timestamptz) |  |  |
| `_nin` | [`[timestamptz!]`](scalars.md#timestamptz) |  |  |

## <a name="tstzrange_comparison_exp"></a>tstzrange_comparison_exp

> Boolean expression to compare columns of type "tstzrange". All fields are combined with logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_eq` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_gt` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_gte` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_in` | [`[tstzrange!]`](scalars.md#tstzrange) |  |  |
| `_is_null` | [`Boolean`](scalars.md#boolean) |  |  |
| `_lt` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_lte` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_neq` | [`tstzrange`](scalars.md#tstzrange) |  |  |
| `_nin` | [`[tstzrange!]`](scalars.md#tstzrange) |  |  |

## <a name="utterances_aggregate_order_by"></a>utterances_aggregate_order_by

> order by aggregate values of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `avg` | [`utterances_avg_order_by`](inputs.md#utterances_avg_order_by) |  |  |
| `count` | [`order_by`](enums.md#order_by) |  |  |
| `max` | [`utterances_max_order_by`](inputs.md#utterances_max_order_by) |  |  |
| `min` | [`utterances_min_order_by`](inputs.md#utterances_min_order_by) |  |  |
| `stddev` | [`utterances_stddev_order_by`](inputs.md#utterances_stddev_order_by) |  |  |
| `stddev_pop` | [`utterances_stddev_pop_order_by`](inputs.md#utterances_stddev_pop_order_by) |  |  |
| `stddev_samp` | [`utterances_stddev_samp_order_by`](inputs.md#utterances_stddev_samp_order_by) |  |  |
| `sum` | [`utterances_sum_order_by`](inputs.md#utterances_sum_order_by) |  |  |
| `var_pop` | [`utterances_var_pop_order_by`](inputs.md#utterances_var_pop_order_by) |  |  |
| `var_samp` | [`utterances_var_samp_order_by`](inputs.md#utterances_var_samp_order_by) |  |  |
| `variance` | [`utterances_variance_order_by`](inputs.md#utterances_variance_order_by) |  |  |

## <a name="utterances_arr_rel_insert_input"></a>utterances_arr_rel_insert_input

> input type for inserting array relation for remote table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `data` | [`[utterances_insert_input!]!`](inputs.md#utterances_insert_input) |  |  |

## <a name="utterances_avg_order_by"></a>utterances_avg_order_by

> order by avg() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_bool_exp"></a>utterances_bool_exp

> Boolean expression to filter rows from the table "utterances". All fields are combined with a logical 'AND'.

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_and` | [`[utterances_bool_exp!]`](inputs.md#utterances_bool_exp) |  |  |
| `_not` | [`utterances_bool_exp`](inputs.md#utterances_bool_exp) |  |  |
| `_or` | [`[utterances_bool_exp!]`](inputs.md#utterances_bool_exp) |  |  |
| `conversation` | [`conversations_bool_exp`](inputs.md#conversations_bool_exp) |  |  |
| `conversation_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `end_user_id` | [`Int_comparison_exp`](inputs.md#int_comparison_exp) |  |  |
| `normalized_utterance` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |
| `speaker_type` | [`speaker_type_enum_enum_comparison_exp`](inputs.md#speaker_type_enum_enum_comparison_exp) |  |  |
| `timestamp` | [`timestamptz_comparison_exp`](inputs.md#timestamptz_comparison_exp) |  |  |
| `utterance` | [`String_comparison_exp`](inputs.md#string_comparison_exp) |  |  |

## <a name="utterances_insert_input"></a>utterances_insert_input

> input type for inserting data into table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation` | [`conversations_obj_rel_insert_input`](inputs.md#conversations_obj_rel_insert_input) |  |  |
| `speaker_type` | [`speaker_type_enum_enum`](enums.md#speaker_type_enum_enum) |  |  |
| `utterance` | [`String`](scalars.md#string) |  |  |

## <a name="utterances_max_order_by"></a>utterances_max_order_by

> order by max() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `normalized_utterance` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |
| `utterance` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_min_order_by"></a>utterances_min_order_by

> order by min() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `normalized_utterance` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |
| `utterance` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_order_by"></a>utterances_order_by

> Ordering options when selecting data from "utterances".

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation` | [`conversations_order_by`](inputs.md#conversations_order_by) |  |  |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |
| `normalized_utterance` | [`order_by`](enums.md#order_by) |  |  |
| `speaker_type` | [`order_by`](enums.md#order_by) |  |  |
| `timestamp` | [`order_by`](enums.md#order_by) |  |  |
| `utterance` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_set_input"></a>utterances_set_input

> input type for updating data in table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `speaker_type` | [`speaker_type_enum_enum`](enums.md#speaker_type_enum_enum) |  |  |
| `utterance` | [`String`](scalars.md#string) |  |  |

## <a name="utterances_stddev_order_by"></a>utterances_stddev_order_by

> order by stddev() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_stddev_pop_order_by"></a>utterances_stddev_pop_order_by

> order by stddev_pop() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_stddev_samp_order_by"></a>utterances_stddev_samp_order_by

> order by stddev_samp() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_sum_order_by"></a>utterances_sum_order_by

> order by sum() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_var_pop_order_by"></a>utterances_var_pop_order_by

> order by var_pop() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_var_samp_order_by"></a>utterances_var_samp_order_by

> order by var_samp() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |

## <a name="utterances_variance_order_by"></a>utterances_variance_order_by

> order by variance() on columns of table "utterances"

### Inputs

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `conversation_id` | [`order_by`](enums.md#order_by) |  |  |
| `end_user_id` | [`order_by`](enums.md#order_by) |  |  |


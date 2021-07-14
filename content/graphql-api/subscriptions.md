# subscription_root

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


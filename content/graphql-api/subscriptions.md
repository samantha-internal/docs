# Subscriptions

## apps

> An array relationship

**Type:** [`[apps!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#apps)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[apps_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#apps_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[apps_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_order_by) | sort the rows by one or more columns |  |
| `where` | [`apps_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_bool_exp) | filter the rows returned |  |

## atomic\_data

> fetch data from the table: "atomic.data"

**Type:** [`[atomic_data!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#atomic_data)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[atomic_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#atomic_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[atomic_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#atomic_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`atomic_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#atomic_data_bool_exp) | filter the rows returned |  |

## atomic\_data\_aggregate

> fetch aggregated fields from the table: "atomic.data"

**Type:** [`atomic_data_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#atomic_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[atomic_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#atomic_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[atomic_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#atomic_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`atomic_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#atomic_data_bool_exp) | filter the rows returned |  |

## conceptnet\_data

> fetch data from the table: "conceptnet.data"

**Type:** [`[conceptnet_data!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conceptnet_data)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[conceptnet_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet\_data\_aggregate

> fetch aggregated fields from the table: "conceptnet.data"

**Type:** [`conceptnet_data_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conceptnet_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[conceptnet_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet\_search\_relations

> execute function "conceptnet.search\_relations" which returns "conceptnet.data"

**Type:** [`[conceptnet_data!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conceptnet_data)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `args` | [`conceptnet_search_relations_args!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_search_relations_args) | input parameters for function "conceptnet.search\_relations" |  |
| `distinct_on` | [`[conceptnet_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conceptnet\_search\_relations\_aggregate

> execute function "conceptnet.search\_relations" and query aggregates on result of table type "conceptnet.data"

**Type:** [`conceptnet_data_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conceptnet_data_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `args` | [`conceptnet_search_relations_args!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_search_relations_args) | input parameters for function "conceptnet.search\_relations" |  |
| `distinct_on` | [`[conceptnet_data_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#conceptnet_data_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[conceptnet_data_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_order_by) | sort the rows by one or more columns |  |
| `where` | [`conceptnet_data_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conceptnet_data_bool_exp) | filter the rows returned |  |

## conversations

> An array relationship

**Type:** [`[conversations!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conversations)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[conversations_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#conversations_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[conversations_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_order_by) | sort the rows by one or more columns |  |
| `where` | [`conversations_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_bool_exp) | filter the rows returned |  |

## developers

> fetch data from the table: "developers"

**Type:** [`[developers!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#developers)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[developers_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[developers_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_bool_exp) | filter the rows returned |  |

## developers\_aggregate

> fetch aggregated fields from the table: "developers"

**Type:** [`developers_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#developers_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[developers_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[developers_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_bool_exp) | filter the rows returned |  |

## events

> An array relationship

**Type:** [`[events!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#events)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[events_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#events_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[events_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#events_order_by) | sort the rows by one or more columns |  |
| `where` | [`events_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#events_bool_exp) | filter the rows returned |  |

## events\_aggregate

> An aggregate relationship

**Type:** [`events_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#events_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[events_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#events_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[events_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#events_order_by) | sort the rows by one or more columns |  |
| `where` | [`events_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#events_bool_exp) | filter the rows returned |  |

## history

> fetch data from the table: "history"

**Type:** [`[history!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#history)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[history_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#history_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[history_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#history_order_by) | sort the rows by one or more columns |  |
| `where` | [`history_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#history_bool_exp) | filter the rows returned |  |

## kv\_store

> An array relationship

**Type:** [`[kv_store!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#kv_store)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[kv_store_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#kv_store_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[kv_store_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#kv_store_order_by) | sort the rows by one or more columns |  |
| `where` | [`kv_store_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#kv_store_bool_exp) | filter the rows returned |  |

## kv\_store\_by\_pk

> fetch data from the table: "kv\_store" using primary key columns

**Type:** [`kv_store`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#kv_store)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `key` | [`String!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#string) |  |  |
| `scope` | [`String!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#string) |  |  |
| `scope_object_id` | [`Int!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) |  |  |

## last\_utterance

> fetch data from the table: "last\_utterance"

**Type:** [`[last_utterance!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#last_utterance)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[last_utterance_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#last_utterance_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[last_utterance_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#last_utterance_order_by) | sort the rows by one or more columns |  |
| `where` | [`last_utterance_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#last_utterance_bool_exp) | filter the rows returned |  |

## me

> execute function "me" which returns "developers"

**Type:** [`[developers!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#developers)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[developers_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[developers_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_bool_exp) | filter the rows returned |  |

## me\_aggregate

> execute function "me" and query aggregates on result of table type "developers"

**Type:** [`developers_aggregate!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#developers_aggregate)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[developers_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#developers_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[developers_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_order_by) | sort the rows by one or more columns |  |
| `where` | [`developers_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_bool_exp) | filter the rows returned |  |

## utterances

> An array relationship

**Type:** [`[utterances!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#utterances)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `distinct_on` | [`[utterances_select_column!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/enums.md#utterances_select_column) | distinct select on columns |  |
| `limit` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | limit the number of rows returned |  |
| `offset` | [`Int`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/scalars.md#int) | skip the first n rows. Use only with order\_by |  |
| `order_by` | [`[utterances_order_by!]`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_order_by) | sort the rows by one or more columns |  |
| `where` | [`utterances_bool_exp`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_bool_exp) | filter the rows returned |  |

\(fin\)


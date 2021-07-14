# mutation_root

> mutation root

## delete_apps

> delete data from the table: "apps"

**Type:** [`apps_mutation_response`](objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `where` | [`apps_bool_exp!`](inputs.md#apps_bool_exp) | filter the rows which have to be deleted |  |

## delete_conversations

> delete data from the table: "conversations"

**Type:** [`conversations_mutation_response`](objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `where` | [`conversations_bool_exp!`](inputs.md#conversations_bool_exp) | filter the rows which have to be deleted |  |

## delete_utterances

> delete data from the table: "utterances"

**Type:** [`utterances_mutation_response`](objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `where` | [`utterances_bool_exp!`](inputs.md#utterances_bool_exp) | filter the rows which have to be deleted |  |

## insert_apps

> insert data into the table: "apps"

**Type:** [`apps_mutation_response`](objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `objects` | [`[apps_insert_input!]!`](inputs.md#apps_insert_input) | the rows to be inserted |  |
| `on_conflict` | [`apps_on_conflict`](inputs.md#apps_on_conflict) | on conflict condition |  |

## insert_apps_one

> insert a single row into the table: "apps"

**Type:** [`apps`](objects.md#apps)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `object` | [`apps_insert_input!`](inputs.md#apps_insert_input) | the row to be inserted |  |
| `on_conflict` | [`apps_on_conflict`](inputs.md#apps_on_conflict) | on conflict condition |  |

## insert_conversations

> insert data into the table: "conversations"

**Type:** [`conversations_mutation_response`](objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `objects` | [`[conversations_insert_input!]!`](inputs.md#conversations_insert_input) | the rows to be inserted |  |
| `on_conflict` | [`conversations_on_conflict`](inputs.md#conversations_on_conflict) | on conflict condition |  |

## insert_conversations_one

> insert a single row into the table: "conversations"

**Type:** [`conversations`](objects.md#conversations)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `object` | [`conversations_insert_input!`](inputs.md#conversations_insert_input) | the row to be inserted |  |
| `on_conflict` | [`conversations_on_conflict`](inputs.md#conversations_on_conflict) | on conflict condition |  |

## insert_utterances

> insert data into the table: "utterances"

**Type:** [`utterances_mutation_response`](objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `objects` | [`[utterances_insert_input!]!`](inputs.md#utterances_insert_input) | the rows to be inserted |  |

## insert_utterances_one

> insert a single row into the table: "utterances"

**Type:** [`utterances`](objects.md#utterances)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `object` | [`utterances_insert_input!`](inputs.md#utterances_insert_input) | the row to be inserted |  |

## update_apps

> update data of the table: "apps"

**Type:** [`apps_mutation_response`](objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_set` | [`apps_set_input`](inputs.md#apps_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`apps_bool_exp!`](inputs.md#apps_bool_exp) | filter the rows which have to be updated |  |

## update_conversations

> update data of the table: "conversations"

**Type:** [`conversations_mutation_response`](objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_set` | [`conversations_set_input`](inputs.md#conversations_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`conversations_bool_exp!`](inputs.md#conversations_bool_exp) | filter the rows which have to be updated |  |

## update_developers

> update data of the table: "developers"

**Type:** [`developers_mutation_response`](objects.md#developers_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_set` | [`developers_set_input`](inputs.md#developers_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`developers_bool_exp!`](inputs.md#developers_bool_exp) | filter the rows which have to be updated |  |

## update_utterances

> update data of the table: "utterances"

**Type:** [`utterances_mutation_response`](objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| --- | --- | --- | --- |
| `_set` | [`utterances_set_input`](inputs.md#utterances_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`utterances_bool_exp!`](inputs.md#utterances_bool_exp) | filter the rows which have to be updated |  |


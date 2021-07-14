# Mutations

> mutation root

## delete\_apps

> delete data from the table: "apps"

**Type:** [`apps_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `where` | [`apps_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_bool_exp) | filter the rows which have to be deleted |  |

## delete\_conversations

> delete data from the table: "conversations"

**Type:** [`conversations_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `where` | [`conversations_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_bool_exp) | filter the rows which have to be deleted |  |

## delete\_utterances

> delete data from the table: "utterances"

**Type:** [`utterances_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `where` | [`utterances_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_bool_exp) | filter the rows which have to be deleted |  |

## insert\_apps

> insert data into the table: "apps"

**Type:** [`apps_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `objects` | [`[apps_insert_input!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_insert_input) | the rows to be inserted |  |
| `on_conflict` | [`apps_on_conflict`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_on_conflict) | on conflict condition |  |

## insert\_apps\_one

> insert a single row into the table: "apps"

**Type:** [`apps`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#apps)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `object` | [`apps_insert_input!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_insert_input) | the row to be inserted |  |
| `on_conflict` | [`apps_on_conflict`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_on_conflict) | on conflict condition |  |

## insert\_conversations

> insert data into the table: "conversations"

**Type:** [`conversations_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `objects` | [`[conversations_insert_input!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_insert_input) | the rows to be inserted |  |
| `on_conflict` | [`conversations_on_conflict`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_on_conflict) | on conflict condition |  |

## insert\_conversations\_one

> insert a single row into the table: "conversations"

**Type:** [`conversations`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conversations)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `object` | [`conversations_insert_input!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_insert_input) | the row to be inserted |  |
| `on_conflict` | [`conversations_on_conflict`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_on_conflict) | on conflict condition |  |

## insert\_utterances

> insert data into the table: "utterances"

**Type:** [`utterances_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `objects` | [`[utterances_insert_input!]!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_insert_input) | the rows to be inserted |  |

## insert\_utterances\_one

> insert a single row into the table: "utterances"

**Type:** [`utterances`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#utterances)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `object` | [`utterances_insert_input!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_insert_input) | the row to be inserted |  |

## update\_apps

> update data of the table: "apps"

**Type:** [`apps_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#apps_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `_set` | [`apps_set_input`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`apps_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#apps_bool_exp) | filter the rows which have to be updated |  |

## update\_conversations

> update data of the table: "conversations"

**Type:** [`conversations_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#conversations_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `_set` | [`conversations_set_input`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`conversations_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#conversations_bool_exp) | filter the rows which have to be updated |  |

## update\_developers

> update data of the table: "developers"

**Type:** [`developers_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#developers_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `_set` | [`developers_set_input`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`developers_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#developers_bool_exp) | filter the rows which have to be updated |  |

## update\_utterances

> update data of the table: "utterances"

**Type:** [`utterances_mutation_response`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/objects.md#utterances_mutation_response)

### Arguments

| Name | Type | Description | Default Value |
| :--- | :--- | :--- | :--- |
| `_set` | [`utterances_set_input`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_set_input) | sets the columns of the filtered rows to the given values |  |
| `where` | [`utterances_bool_exp!`](https://github.com/whitehead-ai/docs/tree/46ddb0dccc2de0fdea4b2a29e0bdee0f1d71d41b/content/graphql-api/inputs.md#utterances_bool_exp) | filter the rows which have to be updated |  |

\(fin\)


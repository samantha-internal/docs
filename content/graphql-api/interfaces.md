# Interfaces

## <a name="container"></a>Container

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

### Implemented by

* `NLUResult`
* `NLUSpan`
* `NLUToken`
* `NlpDoc`
* `Span`
* `Token`


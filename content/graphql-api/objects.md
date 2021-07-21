# Objects

## <a name="aceresult"></a>ACEResult

> Output type

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`String`](scalars.md#string) | APE output |

## <a name="cat"></a>Cat

> Category applied to whole document (label, score), or to spans (start, end, label, score).

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `end` | [`Int`](scalars.md#int) | Span end position |
| `label` | [`String`](scalars.md#string) | Document label |
| `score` | [`Float`](scalars.md#float) | Document score |
| `start` | [`Int`](scalars.md#int) | Span start position |

## <a name="chitchatresponse"></a>ChitchatResponse

> Chitchat results

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`String`](scalars.md#string) |  |

## <a name="classificationresult"></a>ClassificationResult

> Topic classification results

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[TopicScore]`](objects.md#topicscore) |  |

## <a name="composeresult"></a>ComposeResult

> Output result

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`JSON`](scalars.md#json) | Resulting JSON |

## <a name="contextresult"></a>ContextResult

> SLING document container

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `context` | [`SlingDocument`](objects.md#slingdocument) | SLING document |

## <a name="corefcluster"></a>CorefCluster

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `i` | [`Int`](scalars.md#int) | Index of the cluster in the Doc |

## <a name="corefresult"></a>CorefResult

> Coreference resolution data

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `coreferences` | [`[CorefResultScores]`](objects.md#corefresultscores) | Scores of the coreference resolution between mentions. |
| `has_coreference` | [`Boolean`](scalars.md#boolean) | Has any coreference has been resolved in the Doc |
| `result` | [`String`](scalars.md#string) | Unicode representation of the doc where each corefering mention is replaced by the main mention in the associated cluster. |

## <a name="corefresultscores"></a>CorefResultScores

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `mention` | [`String`](scalars.md#string) | Cluster mention |
| `reference` | [`[ResultScores]`](objects.md#resultscores) | Scores of the coreference resolution between mentions. |

## <a name="corefscores"></a>CorefScores

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `mention` | [`String`](scalars.md#string) | Cluster mention |
| `scores` | [`[Scores]`](objects.md#scores) | Scores of the coreference resolution between mentions. |

## <a name="dialogalternative"></a>DialogAlternative

> One of the alternatives, among which the next turn must be chosen

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `alternative` | [`String`](scalars.md#string) | Content of the utterance |
| `score` | [`Float`](scalars.md#float) | Confidence of the utterance |

## <a name="docextension"></a>DocExtension

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `coref_clusters` | [`[CorefCluster]`](objects.md#corefcluster) | All the clusters of corefering mentions in the doc |
| `coref_resolved` | [`String`](scalars.md#string) | Unicode representation of the doc where each corefering mention is replaced by the main mention in the associated cluster. |
| `coref_scores` | [`[CorefScores]`](objects.md#corefscores) | Scores of the coreference resolution between mentions. |
| `has_coref` | [`Boolean`](scalars.md#boolean) | Has any coreference has been resolved in the Doc |

## <a name="matchintentoutput"></a>MatchIntentOutput

> Intent matching output

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[PhraseMatch]`](objects.md#phrasematch) | A list of matches found |
| `warnings` | [`[String]`](scalars.md#string) | A list of processing errors if any |

## <a name="nluresult"></a>NLUResult

> A container for accessing linguistic annotations. Access sentences and named entities.

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `entities` | [`[NLUSpan]`](objects.md#nluspan) | The named entities in the document. Returns a list of named entity Span objects, if the entity recognizer has been applied. |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `noun_chunks` | [`[NLUSpan]`](objects.md#nluspan) | The base noun phrases in the document.    Returns a list of base noun-phrase Span objects, if the document has been syntactically parsed.    A base noun phrase, or “NP chunk”, is a noun phrase that does not permit other NPs to be nested within it – so no NP-level coordination, no prepositional phrases, and no relative clauses. |
| `sentences` | [`[NLUSpan]`](objects.md#nluspan) | The the sentences in the document.    Sentence spans have no label. To improve accuracy on informal texts, spaCy calculates sentence boundaries from the syntactic dependency parse.    If the parser is disabled, the sents iterator will be unavailable. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `tokens` | [`[NLUToken]`](objects.md#nlutoken) | The tokens of the document. |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

## <a name="nluspan"></a>NLUSpan

> A slice from a Doc object

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `entities` | [`[NLUSpan]`](objects.md#nluspan) | Span references |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `lemma` | [`String`](scalars.md#string) | Base form of the span, with no inflectional suffixes. |
| `subtree` | [`[NLUToken]`](objects.md#nlutoken) | Tokens within the span and tokens which descend from them. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `tokens` | [`[NLUToken]`](objects.md#nlutoken) | Token references |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

## <a name="nlutoken"></a>NLUToken

> An individual token — i.e. a word, punctuation symbol, whitespace, etc.

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `dependency` | [`String`](scalars.md#string) | Syntactic dependency relation. |
| `entity_type` | [`String`](scalars.md#string) | Named entity type |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `is_alpha` | [`Boolean`](scalars.md#boolean) | Does the token consist of alphabetic characters? |
| `is_ascii` | [`Boolean`](scalars.md#boolean) | Does the token consist of ASCII characters? |
| `is_bracket` | [`Boolean`](scalars.md#boolean) | Is the token a bracket? |
| `is_currency` | [`Boolean`](scalars.md#boolean) | Is the token a currency symbol? |
| `is_digit` | [`Boolean`](scalars.md#boolean) | Does the token consist of digits? |
| `is_left_punct` | [`Boolean`](scalars.md#boolean) | Is the token a left punctuation mark, e.g. "(" ? |
| `is_lower` | [`Boolean`](scalars.md#boolean) | Is the token in lowercase? |
| `is_oov` | [`Boolean`](scalars.md#boolean) | Is the token out-of-vocabulary (i.e. does it not have a word vector)? |
| `is_punct` | [`Boolean`](scalars.md#boolean) | Is the token punctuation? |
| `is_quote` | [`Boolean`](scalars.md#boolean) | Is the token a quotation mark? |
| `is_right_punct` | [`Boolean`](scalars.md#boolean) | Is the token a right punctuation mark, e.g. ")" ? |
| `is_sent_start` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether the token starts a sentence |
| `is_space` | [`Boolean`](scalars.md#boolean) | Does the token consist of whitespace characters? |
| `is_stop` | [`Boolean`](scalars.md#boolean) | Is the token part of a “stop list”? |
| `is_title` | [`Boolean`](scalars.md#boolean) | Is the token in titlecase? |
| `is_upper` | [`Boolean`](scalars.md#boolean) | Is the token in uppercase? |
| `lemma` | [`String`](scalars.md#string) | Base form of the token, with no inflectional suffixes. |
| `like_email` | [`Boolean`](scalars.md#boolean) | Does the token resemble an email address? |
| `like_num` | [`Boolean`](scalars.md#boolean) | Does the token represent a number? e.g. "10.9", "10", "ten", etc. |
| `like_url` | [`Boolean`](scalars.md#boolean) | Does the token resemble a URL? |
| `log_probability` | [`Float`](scalars.md#float) | Smoothed log probability estimate of token's word type (context-independent entry in the vocabulary). |
| `normalized` | [`String`](scalars.md#string) | The token's norm, i.e. a normalized form of the token text |
| `part_of_speech` | [`String`](scalars.md#string) | Coarse-grained part-of-speech. |
| `subtree` | [`[NLUToken]`](objects.md#nlutoken) | A sequence containing the token and all the token’s syntactic descendants. |
| `tag` | [`String`](scalars.md#string) | Fine-grained part-of-speech. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

## <a name="nlpdoc"></a>NlpDoc

> A container for accessing linguistic annotations. Access sentences and named entities.

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `cats` | [`[Cat]`](objects.md#cat) | List of categories applied to the whole document |
| `ents` | [`[Span]`](objects.md#span) | The named entities in the document. Returns a list of named entity Span objects, if the entity recognizer has been applied. |
| `extension` | [`DocExtension`](objects.md#docextension) |  |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `id` | [`Int`](scalars.md#int) | Document ID |
| `noun_chunks` | [`[Span]`](objects.md#span) | The base noun phrases in the document.    Returns a list of base noun-phrase Span objects, if the document has been syntactically parsed.    A base noun phrase, or “NP chunk”, is a noun phrase that does not permit other NPs to be nested within it – so no NP-level coordination, no prepositional phrases, and no relative clauses. |
| `sentiment` | [`Float`](scalars.md#float) | Sentiment score in the interval from zero to one (negative to positive) |
| `sents` | [`[Span]`](objects.md#span) | The the sentences in the document.    Sentence spans have no label. To improve accuracy on informal texts, spaCy calculates sentence boundaries from the syntactic dependency parse.    If the parser is disabled, the sents iterator will be unavailable. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `tokens` | [`[Token]`](objects.md#token) | The tokens of the document. |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

## <a name="pairsimilarity"></a>PairSimilarity

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `candidate` | [`String`](scalars.md#string) | Similarity sentences pair |
| `input` | [`String`](scalars.md#string) | Similarity sentences pair |
| `score` | [`Float`](scalars.md#float) | Similarity score |

## <a name="paraphrase"></a>Paraphrase

> Paraphrasing results

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[String]`](scalars.md#string) | A list of paraphrases |

## <a name="phrasematch"></a>PhraseMatch

> A phrase match

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `matched_intent` | [`String`](scalars.md#string) | The intent that get a match |
| `similarity` | [`Float`](scalars.md#float) | Similatiry measure |
| `word_matches` | [`[WordMatch]`](objects.md#wordmatch) | A list of word matches |

## <a name="qa_result"></a>QA_Result

> Answer to the given question

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`String!`](scalars.md#string) | Question-answer result |

## <a name="relationresult"></a>RelationResult

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[String]`](scalars.md#string) | Extracted relations |

## <a name="result"></a>Result

> Turn prediction result

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[DialogAlternative]`](objects.md#dialogalternative) | Ranked list of alternatives |

## <a name="resultscores"></a>ResultScores

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `score` | [`Float`](scalars.md#float) | Score of the coreference resolution for this mention |
| `text` | [`String`](scalars.md#string) | Mention text |

## <a name="ssmlresult"></a>SSMLResult

> Output result

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `ssml` | [`String`](scalars.md#string) | Rendered SSML |

## <a name="sttresult"></a>STTResult

> Output result

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `alternatives` | [`[TextAlternative]`](objects.md#textalternative) | A list of alternatives |

## <a name="scores"></a>Scores

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `mention` | [`String`](scalars.md#string) | Mention text |
| `score` | [`Float`](scalars.md#float) | Score of the coreference resolution for this mention |

## <a name="sentencesimilarityscores"></a>SentenceSimilarityScores

> Sentence similarity score

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `result` | [`[PairSimilarity]`](objects.md#pairsimilarity) | A list of pair similarity results |

## <a name="sentimentanalysisresult"></a>SentimentAnalysisResult

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `label` | [`String`](scalars.md#string) | Sentiment label |
| `score` | [`Float`](scalars.md#float) | Sentiment score |

## <a name="serviceinfo"></a>ServiceInfo

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `enums` | [`String`](scalars.md#string) |  |
| `inputs` | [`String`](scalars.md#string) |  |
| `interfaces` | [`String`](scalars.md#string) |  |
| `objects` | [`String`](scalars.md#string) |  |
| `queries` | [`String`](scalars.md#string) |  |
| `scalars` | [`String`](scalars.md#string) |  |
| `schema` | [`String`](scalars.md#string) |  |

## <a name="slingdocument"></a>SlingDocument

> SLING document

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `mentions` | [`[SlingMention]`](objects.md#slingmention) | List of mentions |
| `text` | [`String`](scalars.md#string) | Document text |

## <a name="slingmention"></a>SlingMention

> SLING mention

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `evokes` | [`[String]`](scalars.md#string) | List of words this mention evokes |
| `phrase` | [`String`](scalars.md#string) | Mention phrase |

## <a name="span"></a>Span

> A slice from a Doc object

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `conjuncts` | [`[Token]`](objects.md#token) | A tuple of tokens coordinated to span.root. |
| `end` | [`Int`](scalars.md#int) | End position of the slice |
| `ents` | [`[Span]`](objects.md#span) | Span references |
| `extension` | [`SpanExtension`](objects.md#spanextension) |  |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `label` | [`String`](scalars.md#string) | Span label |
| `lefts` | [`[Token]`](objects.md#token) | Tokens that are to the left of the span, whose heads are within the span. |
| `lemma` | [`String`](scalars.md#string) | Base form of the span, with no inflectional suffixes. |
| `rights` | [`[Token]`](objects.md#token) | Tokens that are to the right of the span, whose heads are within the span. |
| `root` | [`Token`](objects.md#token) | The token with the shortest path to the root of the sentence |
| `start` | [`Int`](scalars.md#int) | Start position of the slice |
| `subtree` | [`[Token]`](objects.md#token) | Tokens within the span and tokens which descend from them. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `tokens` | [`[Token]`](objects.md#token) | Token references |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |

## <a name="spanextension"></a>SpanExtension

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `coref_cluster` | [`CorefCluster`](objects.md#corefcluster) | All the clusters of corefering mentions in the doc |
| `coref_scores` | [`[Scores]`](objects.md#scores) | Scores of the coreference resolution between mentions |
| `is_coref` | [`Boolean`](scalars.md#boolean) | Is the span a coreference? |

## <a name="ttsresult"></a>TTSResult

> Output result

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `audioB64` | [`String`](scalars.md#string) | Resulting audio as a base64 string |

## <a name="textalternative"></a>TextAlternative

> Output text alternative

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `transcript` | [`String`](scalars.md#string) | Output text |

## <a name="token"></a>Token

> An individual token — i.e. a word, punctuation symbol, whitespace, etc.

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `ancestors` | [`[Token]`](objects.md#token) | The rightmost token of this token’s syntactic descendants. |
| `children` | [`[Token]`](objects.md#token) | A sequence of the token’s immediate syntactic children. |
| `cluster` | [`Int`](scalars.md#int) | Brown cluster ID. |
| `conjuncts` | [`[Token]`](objects.md#token) | A tuple of coordinated tokens, not including the token itself. |
| `dep` | [`String`](scalars.md#string) | Syntactic dependency relation. |
| `end` | [`Int`](scalars.md#int) | The ending character offset of the token within the parent document. |
| `ent_iob` | [`String`](scalars.md#string) | IOB code of named entity tag. 3 means the token begins an entity, 2 means it is outside an entity, 1 means it is inside an entity, and 0 means no entity tag is set. |
| `ent_type` | [`String`](scalars.md#string) | Named entity type |
| `extension` | [`TokenExtension`](objects.md#tokenextension) |  |
| `has_vector` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether a word vector is associated with the object. |
| `head` | [`Token`](objects.md#token) | The syntactic parent, or "governor", of this token. |
| `id` | [`Int`](scalars.md#int) | The index of the token within the parent document. |
| `is_alpha` | [`Boolean`](scalars.md#boolean) | Does the token consist of alphabetic characters? |
| `is_ascii` | [`Boolean`](scalars.md#boolean) | Does the token consist of ASCII characters? |
| `is_bracket` | [`Boolean`](scalars.md#boolean) | Is the token a bracket? |
| `is_currency` | [`Boolean`](scalars.md#boolean) | Is the token a currency symbol? |
| `is_digit` | [`Boolean`](scalars.md#boolean) | Does the token consist of digits? |
| `is_left_punct` | [`Boolean`](scalars.md#boolean) | Is the token a left punctuation mark, e.g. "(" ? |
| `is_lower` | [`Boolean`](scalars.md#boolean) | Is the token in lowercase? |
| `is_oov` | [`Boolean`](scalars.md#boolean) | Is the token out-of-vocabulary (i.e. does it not have a word vector)? |
| `is_punct` | [`Boolean`](scalars.md#boolean) | Is the token punctuation? |
| `is_quote` | [`Boolean`](scalars.md#boolean) | Is the token a quotation mark? |
| `is_right_punct` | [`Boolean`](scalars.md#boolean) | Is the token a right punctuation mark, e.g. ")" ? |
| `is_sent_start` | [`Boolean`](scalars.md#boolean) | A boolean value indicating whether the token starts a sentence |
| `is_space` | [`Boolean`](scalars.md#boolean) | Does the token consist of whitespace characters? |
| `is_stop` | [`Boolean`](scalars.md#boolean) | Is the token part of a “stop list”? |
| `is_title` | [`Boolean`](scalars.md#boolean) | Is the token in titlecase? |
| `is_upper` | [`Boolean`](scalars.md#boolean) | Is the token in uppercase? |
| `lang` | [`String`](scalars.md#string) | Language of the parent document’s vocabulary. |
| `left_edge` | [`Token`](objects.md#token) | The leftmost token of this token’s syntactic descendants. |
| `lefts` | [`[Token]`](objects.md#token) | The leftward immediate children of the word in the syntactic dependency parse. |
| `lemma` | [`String`](scalars.md#string) | Base form of the token, with no inflectional suffixes. |
| `like_email` | [`Boolean`](scalars.md#boolean) | Does the token resemble an email address? |
| `like_num` | [`Boolean`](scalars.md#boolean) | Does the token represent a number? e.g. "10.9", "10", "ten", etc. |
| `like_url` | [`Boolean`](scalars.md#boolean) | Does the token resemble a URL? |
| `lower` | [`String`](scalars.md#string) | Lowercase form of the token |
| `norm` | [`String`](scalars.md#string) | The token's norm, i.e. a normalized form of the token text |
| `orth` | [`String`](scalars.md#string) | Verbatim text content (identical to Token.text).    Exists mostly for consistency with the other attributes. |
| `pos` | [`String`](scalars.md#string) | Coarse-grained part-of-speech. |
| `prefix` | [`String`](scalars.md#string) | Hash value of a length-N substring from the start of the token |
| `prob` | [`Float`](scalars.md#float) | Smoothed log probability estimate of token's word type (context-independent entry in the vocabulary). |
| `right_edge` | [`Token`](objects.md#token) | The rightmost token of this token’s syntactic descendants. |
| `rights` | [`[Token]`](objects.md#token) | The rightward immediate children of the word in the syntactic dependency parse. |
| `shape` | [`String`](scalars.md#string) | Transform of the tokens’s string to show orthographic features. Alphabetic characters are replaced by x or X, and numeric characters are replaced by d, and sequences of the same character are truncated after length 4. For example,"Xxxx"or"dd" |
| `start` | [`Int`](scalars.md#int) | The starting character offset of the token within the parent document. |
| `subtree` | [`[Token]`](objects.md#token) | A sequence containing the token and all the token’s syntactic descendants. |
| `suffix` | [`String`](scalars.md#string) | Hash value of a length-N substring from the end of the token |
| `tag` | [`String`](scalars.md#string) | Fine-grained part-of-speech. |
| `text` | [`String`](scalars.md#string) | Verbatim text content. |
| `text_with_ws` | [`String`](scalars.md#string) | Text content, with trailing space character if present. |
| `vector` | [`[Float]`](scalars.md#float) | A real-valued meaning representation. |
| `vector_norm` | [`Float`](scalars.md#float) | The L2 norm of the document’s vector representation. |
| `whitespace` | [`String`](scalars.md#string) | Trailing space character if present |

## <a name="tokenextension"></a>TokenExtension

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `coref_clusters` | [`[CorefCluster]`](objects.md#corefcluster) | All the clusters of corefering mentions in the doc |
| `in_coref` | [`Boolean`](scalars.md#boolean) | Is the token in coreference? |
| `is_implicit` | [`Boolean`](scalars.md#boolean) | Is the token an implicit fused-head? |

## <a name="topicscore"></a>TopicScore

> Topic scores

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `score` | [`Float!`](scalars.md#float) |  |
| `topic` | [`String!`](scalars.md#string) |  |

## <a name="wordmatch"></a>WordMatch

> A word match

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `explanation` | [`String`](scalars.md#string) | Match explanation |
| `extracted_word` | [`String`](scalars.md#string) | A word extracted by the match |
| `match_type` | [`String`](scalars.md#string) | Type of the match |
| `similarity` | [`Float`](scalars.md#float) | Similarity measure |
| `slot` | [`String`](scalars.md#string) | Slot filled by the match |

## <a name="__directive"></a>__Directive

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `args` | [`__InputValue`](objects.md#__inputvalue) |  |
| `description` | [`String!`](scalars.md#string) |  |
| `isRepeatable` | [`String!`](scalars.md#string) |  |
| `locations` | [`String!`](scalars.md#string) |  |
| `name` | [`String!`](scalars.md#string) |  |

## <a name="__enumvalue"></a>__EnumValue

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `deprecationReason` | [`String!`](scalars.md#string) |  |
| `description` | [`String!`](scalars.md#string) |  |
| `isDeprecated` | [`String!`](scalars.md#string) |  |
| `name` | [`String!`](scalars.md#string) |  |

## <a name="__field"></a>__Field

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `args` | [`__InputValue`](objects.md#__inputvalue) |  |
| `deprecationReason` | [`String!`](scalars.md#string) |  |
| `description` | [`String!`](scalars.md#string) |  |
| `isDeprecated` | [`String!`](scalars.md#string) |  |
| `name` | [`String!`](scalars.md#string) |  |
| `type` | [`__Type`](objects.md#__type) |  |

## <a name="__inputvalue"></a>__InputValue

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `defaultValue` | [`String!`](scalars.md#string) |  |
| `description` | [`String!`](scalars.md#string) |  |
| `name` | [`String!`](scalars.md#string) |  |
| `type` | [`__Type`](objects.md#__type) |  |

## <a name="__schema"></a>__Schema

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `description` | [`String!`](scalars.md#string) |  |
| `directives` | [`__Directive`](objects.md#__directive) |  |
| `mutationType` | [`__Type`](objects.md#__type) |  |
| `queryType` | [`__Type`](objects.md#__type) |  |
| `subscriptionType` | [`__Type`](objects.md#__type) |  |
| `types` | [`__Type`](objects.md#__type) |  |

## <a name="__type"></a>__Type

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `description` | [`String!`](scalars.md#string) |  |
| `enumValues` | [`__EnumValue`](objects.md#__enumvalue) |  |
| `fields` | [`__Field`](objects.md#__field) |  |
| `inputFields` | [`__InputValue`](objects.md#__inputvalue) |  |
| `interfaces` | [`__Type`](objects.md#__type) |  |
| `kind` | [`__TypeKind!`](enums.md#__typekind) |  |
| `name` | [`String!`](scalars.md#string) |  |
| `ofType` | [`__Type`](objects.md#__type) |  |
| `possibleTypes` | [`__Type`](objects.md#__type) |  |

## <a name="apps"></a>apps

> columns and relationships of "apps"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `conversations` | [`[conversations!]!`](objects.md#conversations) | An array relationship |
| `created_at` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `developer` | [`developers!`](objects.md#developers) | An object relationship |
| `developer_id` | [`Int!`](scalars.md#int) |  |
| `kv_store` | [`[kv_store!]!`](objects.md#kv_store) | An array relationship |
| `metadata` | [`jsonb!`](scalars.md#jsonb) |  |
| `object_id` | [`Int!`](scalars.md#int) |  |
| `scope_name` | [`String`](scalars.md#string) |  |
| `slug` | [`String!`](scalars.md#string) |  |
| `status` | [`app_status!`](scalars.md#app_status) |  |

## <a name="apps_mutation_response"></a>apps_mutation_response

> response of any mutation on the table "apps"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `affected_rows` | [`Int!`](scalars.md#int) | number of rows affected by the mutation |
| `returning` | [`[apps!]!`](objects.md#apps) | data from the rows affected by the mutation |

## <a name="atomic_data"></a>atomic_data

> columns and relationships of "atomic.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `event` | [`String`](scalars.md#string) |  |
| `o_effect` | [`_text`](scalars.md#_text) |  |
| `o_react` | [`_text`](scalars.md#_text) |  |
| `o_want` | [`_text`](scalars.md#_text) |  |
| `prefix` | [`_text`](scalars.md#_text) |  |
| `x_attr` | [`_text`](scalars.md#_text) |  |
| `x_effect` | [`_text`](scalars.md#_text) |  |
| `x_intent` | [`_text`](scalars.md#_text) |  |
| `x_need` | [`_text`](scalars.md#_text) |  |
| `x_react` | [`_text`](scalars.md#_text) |  |
| `x_want` | [`_text`](scalars.md#_text) |  |

## <a name="atomic_data_aggregate"></a>atomic_data_aggregate

> aggregated selection of "atomic.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `aggregate` | [`atomic_data_aggregate_fields`](objects.md#atomic_data_aggregate_fields) |  |
| `nodes` | [`[atomic_data!]!`](objects.md#atomic_data) |  |

## <a name="atomic_data_aggregate_fields"></a>atomic_data_aggregate_fields

> aggregate fields of "atomic.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `count` | [`Int!`](scalars.md#int) |  |
| `max` | [`atomic_data_max_fields`](objects.md#atomic_data_max_fields) |  |
| `min` | [`atomic_data_min_fields`](objects.md#atomic_data_min_fields) |  |

## <a name="atomic_data_max_fields"></a>atomic_data_max_fields

> aggregate max on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `event` | [`String`](scalars.md#string) |  |

## <a name="atomic_data_min_fields"></a>atomic_data_min_fields

> aggregate min on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `event` | [`String`](scalars.md#string) |  |

## <a name="conceptnet_data"></a>conceptnet_data

> columns and relationships of "conceptnet.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `end` | [`String!`](scalars.md#string) |  |
| `relation` | [`String!`](scalars.md#string) |  |
| `start` | [`String!`](scalars.md#string) |  |
| `uri` | [`String!`](scalars.md#string) |  |
| `weight` | [`numeric!`](scalars.md#numeric) |  |

## <a name="conceptnet_data_aggregate"></a>conceptnet_data_aggregate

> aggregated selection of "conceptnet.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `aggregate` | [`conceptnet_data_aggregate_fields`](objects.md#conceptnet_data_aggregate_fields) |  |
| `nodes` | [`[conceptnet_data!]!`](objects.md#conceptnet_data) |  |

## <a name="conceptnet_data_aggregate_fields"></a>conceptnet_data_aggregate_fields

> aggregate fields of "conceptnet.data"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `avg` | [`conceptnet_data_avg_fields`](objects.md#conceptnet_data_avg_fields) |  |
| `count` | [`Int!`](scalars.md#int) |  |
| `max` | [`conceptnet_data_max_fields`](objects.md#conceptnet_data_max_fields) |  |
| `min` | [`conceptnet_data_min_fields`](objects.md#conceptnet_data_min_fields) |  |
| `stddev` | [`conceptnet_data_stddev_fields`](objects.md#conceptnet_data_stddev_fields) |  |
| `stddev_pop` | [`conceptnet_data_stddev_pop_fields`](objects.md#conceptnet_data_stddev_pop_fields) |  |
| `stddev_samp` | [`conceptnet_data_stddev_samp_fields`](objects.md#conceptnet_data_stddev_samp_fields) |  |
| `sum` | [`conceptnet_data_sum_fields`](objects.md#conceptnet_data_sum_fields) |  |
| `var_pop` | [`conceptnet_data_var_pop_fields`](objects.md#conceptnet_data_var_pop_fields) |  |
| `var_samp` | [`conceptnet_data_var_samp_fields`](objects.md#conceptnet_data_var_samp_fields) |  |
| `variance` | [`conceptnet_data_variance_fields`](objects.md#conceptnet_data_variance_fields) |  |

## <a name="conceptnet_data_avg_fields"></a>conceptnet_data_avg_fields

> aggregate avg on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_max_fields"></a>conceptnet_data_max_fields

> aggregate max on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `end` | [`String`](scalars.md#string) |  |
| `relation` | [`String`](scalars.md#string) |  |
| `start` | [`String`](scalars.md#string) |  |
| `uri` | [`String`](scalars.md#string) |  |
| `weight` | [`numeric`](scalars.md#numeric) |  |

## <a name="conceptnet_data_min_fields"></a>conceptnet_data_min_fields

> aggregate min on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `end` | [`String`](scalars.md#string) |  |
| `relation` | [`String`](scalars.md#string) |  |
| `start` | [`String`](scalars.md#string) |  |
| `uri` | [`String`](scalars.md#string) |  |
| `weight` | [`numeric`](scalars.md#numeric) |  |

## <a name="conceptnet_data_stddev_fields"></a>conceptnet_data_stddev_fields

> aggregate stddev on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_stddev_pop_fields"></a>conceptnet_data_stddev_pop_fields

> aggregate stddev_pop on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_stddev_samp_fields"></a>conceptnet_data_stddev_samp_fields

> aggregate stddev_samp on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_sum_fields"></a>conceptnet_data_sum_fields

> aggregate sum on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`numeric`](scalars.md#numeric) |  |

## <a name="conceptnet_data_var_pop_fields"></a>conceptnet_data_var_pop_fields

> aggregate var_pop on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_var_samp_fields"></a>conceptnet_data_var_samp_fields

> aggregate var_samp on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conceptnet_data_variance_fields"></a>conceptnet_data_variance_fields

> aggregate variance on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `weight` | [`Float`](scalars.md#float) |  |

## <a name="conversations"></a>conversations

> columns and relationships of "conversations"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `app` | [`apps!`](objects.md#apps) | An object relationship |
| `app_id` | [`Int!`](scalars.md#int) |  |
| `created_at` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `destroyed_at` | [`timestamptz`](scalars.md#timestamptz) |  |
| `end_user_id` | [`Int!`](scalars.md#int) |  |
| `kv_store` | [`[kv_store!]!`](objects.md#kv_store) | An array relationship |
| `metadata` | [`jsonb!`](scalars.md#jsonb) |  |
| `object_id` | [`Int!`](scalars.md#int) |  |
| `scope_name` | [`String`](scalars.md#string) |  |
| `utterances` | [`[utterances!]!`](objects.md#utterances) | An array relationship |

## <a name="conversations_mutation_response"></a>conversations_mutation_response

> response of any mutation on the table "conversations"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `affected_rows` | [`Int!`](scalars.md#int) | number of rows affected by the mutation |
| `returning` | [`[conversations!]!`](objects.md#conversations) | data from the rows affected by the mutation |

## <a name="developers"></a>developers

> columns and relationships of "developers"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `active` | [`Boolean!`](scalars.md#boolean) |  |
| `api_key` | [`String!`](scalars.md#string) |  |
| `apps` | [`[apps!]!`](objects.md#apps) | An array relationship |
| `created_at` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `email` | [`String!`](scalars.md#string) |  |
| `events` | [`[events!]!`](objects.md#events) | An array relationship |
| `events_aggregate` | [`events_aggregate!`](objects.md#events_aggregate) | An aggregate relationship |
| `github_handle` | [`String`](scalars.md#string) |  |
| `kv_stores` | [`[kv_store!]!`](objects.md#kv_store) | An array relationship |
| `metadata` | [`jsonb!`](scalars.md#jsonb) |  |
| `name` | [`String!`](scalars.md#string) |  |
| `object_id` | [`Int!`](scalars.md#int) |  |
| `onboarded` | [`Boolean!`](scalars.md#boolean) |  |
| `uid` | [`String!`](scalars.md#string) |  |

## <a name="developers_aggregate"></a>developers_aggregate

> aggregated selection of "developers"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `aggregate` | [`developers_aggregate_fields`](objects.md#developers_aggregate_fields) |  |
| `nodes` | [`[developers!]!`](objects.md#developers) |  |

## <a name="developers_aggregate_fields"></a>developers_aggregate_fields

> aggregate fields of "developers"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `avg` | [`developers_avg_fields`](objects.md#developers_avg_fields) |  |
| `count` | [`Int!`](scalars.md#int) |  |
| `max` | [`developers_max_fields`](objects.md#developers_max_fields) |  |
| `min` | [`developers_min_fields`](objects.md#developers_min_fields) |  |
| `stddev` | [`developers_stddev_fields`](objects.md#developers_stddev_fields) |  |
| `stddev_pop` | [`developers_stddev_pop_fields`](objects.md#developers_stddev_pop_fields) |  |
| `stddev_samp` | [`developers_stddev_samp_fields`](objects.md#developers_stddev_samp_fields) |  |
| `sum` | [`developers_sum_fields`](objects.md#developers_sum_fields) |  |
| `var_pop` | [`developers_var_pop_fields`](objects.md#developers_var_pop_fields) |  |
| `var_samp` | [`developers_var_samp_fields`](objects.md#developers_var_samp_fields) |  |
| `variance` | [`developers_variance_fields`](objects.md#developers_variance_fields) |  |

## <a name="developers_avg_fields"></a>developers_avg_fields

> aggregate avg on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_max_fields"></a>developers_max_fields

> aggregate max on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `api_key` | [`String`](scalars.md#string) |  |
| `created_at` | [`timestamptz`](scalars.md#timestamptz) |  |
| `email` | [`String`](scalars.md#string) |  |
| `github_handle` | [`String`](scalars.md#string) |  |
| `name` | [`String`](scalars.md#string) |  |
| `object_id` | [`Int`](scalars.md#int) |  |
| `uid` | [`String`](scalars.md#string) |  |

## <a name="developers_min_fields"></a>developers_min_fields

> aggregate min on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `api_key` | [`String`](scalars.md#string) |  |
| `created_at` | [`timestamptz`](scalars.md#timestamptz) |  |
| `email` | [`String`](scalars.md#string) |  |
| `github_handle` | [`String`](scalars.md#string) |  |
| `name` | [`String`](scalars.md#string) |  |
| `object_id` | [`Int`](scalars.md#int) |  |
| `uid` | [`String`](scalars.md#string) |  |

## <a name="developers_mutation_response"></a>developers_mutation_response

> response of any mutation on the table "developers"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `affected_rows` | [`Int!`](scalars.md#int) | number of rows affected by the mutation |
| `returning` | [`[developers!]!`](objects.md#developers) | data from the rows affected by the mutation |

## <a name="developers_stddev_fields"></a>developers_stddev_fields

> aggregate stddev on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_stddev_pop_fields"></a>developers_stddev_pop_fields

> aggregate stddev_pop on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_stddev_samp_fields"></a>developers_stddev_samp_fields

> aggregate stddev_samp on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_sum_fields"></a>developers_sum_fields

> aggregate sum on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Int`](scalars.md#int) |  |

## <a name="developers_var_pop_fields"></a>developers_var_pop_fields

> aggregate var_pop on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_var_samp_fields"></a>developers_var_samp_fields

> aggregate var_samp on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="developers_variance_fields"></a>developers_variance_fields

> aggregate variance on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `object_id` | [`Float`](scalars.md#float) |  |

## <a name="events"></a>events

> columns and relationships of "events"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `action` | [`String`](scalars.md#string) |  |
| `changed_fields` | [`jsonb`](scalars.md#jsonb) |  |
| `developer_id` | [`String`](scalars.md#string) |  |
| `table` | [`String`](scalars.md#string) |  |
| `timestamp` | [`timestamptz`](scalars.md#timestamptz) |  |

## <a name="events_aggregate"></a>events_aggregate

> aggregated selection of "events"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `aggregate` | [`events_aggregate_fields`](objects.md#events_aggregate_fields) |  |
| `nodes` | [`[events!]!`](objects.md#events) |  |

## <a name="events_aggregate_fields"></a>events_aggregate_fields

> aggregate fields of "events"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `count` | [`Int!`](scalars.md#int) |  |
| `max` | [`events_max_fields`](objects.md#events_max_fields) |  |
| `min` | [`events_min_fields`](objects.md#events_min_fields) |  |

## <a name="events_max_fields"></a>events_max_fields

> aggregate max on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `action` | [`String`](scalars.md#string) |  |
| `developer_id` | [`String`](scalars.md#string) |  |
| `table` | [`String`](scalars.md#string) |  |
| `timestamp` | [`timestamptz`](scalars.md#timestamptz) |  |

## <a name="events_min_fields"></a>events_min_fields

> aggregate min on columns

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `action` | [`String`](scalars.md#string) |  |
| `developer_id` | [`String`](scalars.md#string) |  |
| `table` | [`String`](scalars.md#string) |  |
| `timestamp` | [`timestamptz`](scalars.md#timestamptz) |  |

## <a name="history"></a>history

> columns and relationships of "history"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `conversation` | [`conversations`](objects.md#conversations) | An object relationship |
| `conversation_id` | [`Int`](scalars.md#int) |  |
| `interval` | [`timestamptz`](scalars.md#timestamptz) |  |
| `updated_at` | [`timestamptz`](scalars.md#timestamptz) |  |
| `utterances` | [`jsonb`](scalars.md#jsonb) |  |
| `window` | [`tstzrange`](scalars.md#tstzrange) |  |

## <a name="kv_store"></a>kv_store

> columns and relationships of "kv_store"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `created_at` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `created_by` | [`Int!`](scalars.md#int) |  |
| `developer` | [`developers!`](objects.md#developers) | An object relationship |
| `key` | [`String!`](scalars.md#string) |  |
| `metadata` | [`jsonb!`](scalars.md#jsonb) |  |
| `object_id` | [`Int!`](scalars.md#int) |  |
| `scope` | [`String!`](scalars.md#string) |  |
| `scope_object_id` | [`Int!`](scalars.md#int) |  |
| `updated_at` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `value` | [`jsonb!`](scalars.md#jsonb) |  |

## <a name="last_utterance"></a>last_utterance

> columns and relationships of "last_utterance"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `conversation` | [`conversations`](objects.md#conversations) | An object relationship |
| `conversation_id` | [`Int`](scalars.md#int) |  |
| `interval` | [`timestamptz`](scalars.md#timestamptz) |  |
| `speaker_type` | [`String`](scalars.md#string) |  |
| `updated_at` | [`timestamptz`](scalars.md#timestamptz) |  |
| `utterance` | [`String`](scalars.md#string) |  |

## <a name="mutation_root"></a>mutation_root

> mutation root

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `delete_apps` | [`apps_mutation_response`](objects.md#apps_mutation_response) | delete data from the table: "apps" |
| `delete_conversations` | [`conversations_mutation_response`](objects.md#conversations_mutation_response) | delete data from the table: "conversations" |
| `delete_utterances` | [`utterances_mutation_response`](objects.md#utterances_mutation_response) | delete data from the table: "utterances" |
| `insert_apps` | [`apps_mutation_response`](objects.md#apps_mutation_response) | insert data into the table: "apps" |
| `insert_apps_one` | [`apps`](objects.md#apps) | insert a single row into the table: "apps" |
| `insert_conversations` | [`conversations_mutation_response`](objects.md#conversations_mutation_response) | insert data into the table: "conversations" |
| `insert_conversations_one` | [`conversations`](objects.md#conversations) | insert a single row into the table: "conversations" |
| `insert_utterances` | [`utterances_mutation_response`](objects.md#utterances_mutation_response) | insert data into the table: "utterances" |
| `insert_utterances_one` | [`utterances`](objects.md#utterances) | insert a single row into the table: "utterances" |
| `update_apps` | [`apps_mutation_response`](objects.md#apps_mutation_response) | update data of the table: "apps" |
| `update_conversations` | [`conversations_mutation_response`](objects.md#conversations_mutation_response) | update data of the table: "conversations" |
| `update_developers` | [`developers_mutation_response`](objects.md#developers_mutation_response) | update data of the table: "developers" |
| `update_utterances` | [`utterances_mutation_response`](objects.md#utterances_mutation_response) | update data of the table: "utterances" |

## <a name="query_root"></a>query_root

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `apps` | [`[apps!]!`](objects.md#apps) | An array relationship |
| `atomic_data` | [`[atomic_data!]!`](objects.md#atomic_data) | fetch data from the table: "atomic.data" |
| `atomic_data_aggregate` | [`atomic_data_aggregate!`](objects.md#atomic_data_aggregate) | fetch aggregated fields from the table: "atomic.data" |
| `callApplyVoiceCSS` | [`SSMLResult`](objects.md#ssmlresult) | Apply voice CSS to the SSML input |
| `callChitchat` | [`ChitchatResponse`](objects.md#chitchatresponse) | Perform chit chat |
| `callClassifyTopic` | [`ClassificationResult`](objects.md#classificationresult) | Classify topics |
| `callCommonsense` | [`RelationResult`](objects.md#relationresult) | Predict category |
| `callCompose` | [`ComposeResult`](objects.md#composeresult) | Execute composition pipeline |
| `callMatchIntent` | [`MatchIntentOutput`](objects.md#matchintentoutput) | Call the intent matching functionality |
| `callMeasureSimilarity` | [`SentenceSimilarityScores`](objects.md#sentencesimilarityscores) | Measure sentences similarity |
| `callNLU` | [`NLUResult`](objects.md#nluresult) | Document processing |
| `callNextDialogTurn` | [`Result`](objects.md#result) | Perform next dialog turn prediction |
| `callParaphraseSentence` | [`Paraphrase`](objects.md#paraphrase) | Perform sentence paraphrasing |
| `callParseACE` | [`ACEResult`](objects.md#aceresult) | Parse ACE sentence |
| `callParseContext` | [`[ContextResult]`](objects.md#contextresult) | Parse frame semantics for a list of dialog turns |
| `callPredictRelation` | [`RelationResult`](objects.md#relationresult) | Predict relations |
| `callQA` | [`QA_Result`](objects.md#qa_result) | Answer questions based on context |
| `callResolveCoreference` | [`CorefResult`](objects.md#corefresult) | Coreference resolution |
| `callSentimentAnalysis` | [`[SentimentAnalysisResult]`](objects.md#sentimentanalysisresult) | Sentiment analisys |
| `callShowDocs` | [`ServiceInfo`](objects.md#serviceinfo) |  |
| `callSpeechToText` | [`[STTResult]`](objects.md#sttresult) | Convert speech to text |
| `callTextToSpeech` | [`TTSResult`](objects.md#ttsresult) | Convert text to speech |
| `conceptnet_data` | [`[conceptnet_data!]!`](objects.md#conceptnet_data) | fetch data from the table: "conceptnet.data" |
| `conceptnet_data_aggregate` | [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate) | fetch aggregated fields from the table: "conceptnet.data" |
| `conceptnet_search_relations` | [`[conceptnet_data!]!`](objects.md#conceptnet_data) | execute function "conceptnet.search_relations" which returns "conceptnet.data" |
| `conceptnet_search_relations_aggregate` | [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate) | execute function "conceptnet.search_relations" and query aggregates on result of table type "conceptnet.data" |
| `conversations` | [`[conversations!]!`](objects.md#conversations) | An array relationship |
| `deprecatedCallNlpDoc` | [`NlpDoc`](objects.md#nlpdoc) | Document processing |
| `developers` | [`[developers!]!`](objects.md#developers) | fetch data from the table: "developers" |
| `developers_aggregate` | [`developers_aggregate!`](objects.md#developers_aggregate) | fetch aggregated fields from the table: "developers" |
| `events` | [`[events!]!`](objects.md#events) | An array relationship |
| `events_aggregate` | [`events_aggregate!`](objects.md#events_aggregate) | An aggregate relationship |
| `history` | [`[history!]!`](objects.md#history) | fetch data from the table: "history" |
| `kv_store` | [`[kv_store!]!`](objects.md#kv_store) | An array relationship |
| `kv_store_by_pk` | [`kv_store`](objects.md#kv_store) | fetch data from the table: "kv_store" using primary key columns |
| `last_utterance` | [`[last_utterance!]!`](objects.md#last_utterance) | fetch data from the table: "last_utterance" |
| `me` | [`[developers!]!`](objects.md#developers) | execute function "me" which returns "developers" |
| `me_aggregate` | [`developers_aggregate!`](objects.md#developers_aggregate) | execute function "me" and query aggregates on result of table type "developers" |
| `utterances` | [`[utterances!]!`](objects.md#utterances) | An array relationship |

## <a name="subscription_root"></a>subscription_root

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `apps` | [`[apps!]!`](objects.md#apps) | An array relationship |
| `atomic_data` | [`[atomic_data!]!`](objects.md#atomic_data) | fetch data from the table: "atomic.data" |
| `atomic_data_aggregate` | [`atomic_data_aggregate!`](objects.md#atomic_data_aggregate) | fetch aggregated fields from the table: "atomic.data" |
| `conceptnet_data` | [`[conceptnet_data!]!`](objects.md#conceptnet_data) | fetch data from the table: "conceptnet.data" |
| `conceptnet_data_aggregate` | [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate) | fetch aggregated fields from the table: "conceptnet.data" |
| `conceptnet_search_relations` | [`[conceptnet_data!]!`](objects.md#conceptnet_data) | execute function "conceptnet.search_relations" which returns "conceptnet.data" |
| `conceptnet_search_relations_aggregate` | [`conceptnet_data_aggregate!`](objects.md#conceptnet_data_aggregate) | execute function "conceptnet.search_relations" and query aggregates on result of table type "conceptnet.data" |
| `conversations` | [`[conversations!]!`](objects.md#conversations) | An array relationship |
| `developers` | [`[developers!]!`](objects.md#developers) | fetch data from the table: "developers" |
| `developers_aggregate` | [`developers_aggregate!`](objects.md#developers_aggregate) | fetch aggregated fields from the table: "developers" |
| `events` | [`[events!]!`](objects.md#events) | An array relationship |
| `events_aggregate` | [`events_aggregate!`](objects.md#events_aggregate) | An aggregate relationship |
| `history` | [`[history!]!`](objects.md#history) | fetch data from the table: "history" |
| `kv_store` | [`[kv_store!]!`](objects.md#kv_store) | An array relationship |
| `kv_store_by_pk` | [`kv_store`](objects.md#kv_store) | fetch data from the table: "kv_store" using primary key columns |
| `last_utterance` | [`[last_utterance!]!`](objects.md#last_utterance) | fetch data from the table: "last_utterance" |
| `me` | [`[developers!]!`](objects.md#developers) | execute function "me" which returns "developers" |
| `me_aggregate` | [`developers_aggregate!`](objects.md#developers_aggregate) | execute function "me" and query aggregates on result of table type "developers" |
| `utterances` | [`[utterances!]!`](objects.md#utterances) | An array relationship |

## <a name="utterances"></a>utterances

> columns and relationships of "utterances"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `conversation` | [`conversations!`](objects.md#conversations) | An object relationship |
| `conversation_id` | [`Int!`](scalars.md#int) |  |
| `end_user_id` | [`Int`](scalars.md#int) |  |
| `normalized_utterance` | [`String!`](scalars.md#string) |  |
| `speaker_type` | [`speaker_type_enum_enum!`](enums.md#speaker_type_enum_enum) |  |
| `timestamp` | [`timestamptz!`](scalars.md#timestamptz) |  |
| `utterance` | [`String!`](scalars.md#string) |  |

## <a name="utterances_mutation_response"></a>utterances_mutation_response

> response of any mutation on the table "utterances"

### Fields

| Name | Type | Description |
| --- | --- | --- |
| `affected_rows` | [`Int!`](scalars.md#int) | number of rows affected by the mutation |
| `returning` | [`[utterances!]!`](objects.md#utterances) | data from the rows affected by the mutation |


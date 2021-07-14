# Schema Types

<details>
  <summary><strong>Table of Contents</strong></summary>

  * [Query](#query)
  * [Mutation](#mutation)
  * [Objects](#objects)
    * [ACEResult](#aceresult)
    * [Cat](#cat)
    * [ChitchatResponse](#chitchatresponse)
    * [ClassificationResult](#classificationresult)
    * [ComposeResult](#composeresult)
    * [ContextResult](#contextresult)
    * [CorefCluster](#corefcluster)
    * [CorefResult](#corefresult)
    * [CorefResultScores](#corefresultscores)
    * [CorefScores](#corefscores)
    * [DialogAlternative](#dialogalternative)
    * [DocExtension](#docextension)
    * [MatchIntentOutput](#matchintentoutput)
    * [NLUResult](#nluresult)
    * [NLUSpan](#nluspan)
    * [NLUToken](#nlutoken)
    * [NlpDoc](#nlpdoc)
    * [PairSimilarity](#pairsimilarity)
    * [Paraphrase](#paraphrase)
    * [PhraseMatch](#phrasematch)
    * [QA_Result](#qa_result)
    * [RelationResult](#relationresult)
    * [Result](#result)
    * [ResultScores](#resultscores)
    * [SSMLResult](#ssmlresult)
    * [STTResult](#sttresult)
    * [Scores](#scores)
    * [SentenceSimilarityScores](#sentencesimilarityscores)
    * [SentimentAnalysisResult](#sentimentanalysisresult)
    * [ServiceInfo](#serviceinfo)
    * [SlingDocument](#slingdocument)
    * [SlingMention](#slingmention)
    * [Span](#span)
    * [SpanExtension](#spanextension)
    * [TTSResult](#ttsresult)
    * [TextAlternative](#textalternative)
    * [Token](#token)
    * [TokenExtension](#tokenextension)
    * [TopicScore](#topicscore)
    * [WordMatch](#wordmatch)
    * [apps](#apps)
    * [apps_aggregate](#apps_aggregate)
    * [apps_aggregate_fields](#apps_aggregate_fields)
    * [apps_avg_fields](#apps_avg_fields)
    * [apps_max_fields](#apps_max_fields)
    * [apps_min_fields](#apps_min_fields)
    * [apps_mutation_response](#apps_mutation_response)
    * [apps_stddev_fields](#apps_stddev_fields)
    * [apps_stddev_pop_fields](#apps_stddev_pop_fields)
    * [apps_stddev_samp_fields](#apps_stddev_samp_fields)
    * [apps_sum_fields](#apps_sum_fields)
    * [apps_var_pop_fields](#apps_var_pop_fields)
    * [apps_var_samp_fields](#apps_var_samp_fields)
    * [apps_variance_fields](#apps_variance_fields)
    * [atomic_data](#atomic_data)
    * [atomic_data_aggregate](#atomic_data_aggregate)
    * [atomic_data_aggregate_fields](#atomic_data_aggregate_fields)
    * [atomic_data_max_fields](#atomic_data_max_fields)
    * [atomic_data_min_fields](#atomic_data_min_fields)
    * [atomic_data_mutation_response](#atomic_data_mutation_response)
    * [audit_logged_actions](#audit_logged_actions)
    * [audit_logged_actions_aggregate](#audit_logged_actions_aggregate)
    * [audit_logged_actions_aggregate_fields](#audit_logged_actions_aggregate_fields)
    * [audit_logged_actions_avg_fields](#audit_logged_actions_avg_fields)
    * [audit_logged_actions_max_fields](#audit_logged_actions_max_fields)
    * [audit_logged_actions_min_fields](#audit_logged_actions_min_fields)
    * [audit_logged_actions_mutation_response](#audit_logged_actions_mutation_response)
    * [audit_logged_actions_stddev_fields](#audit_logged_actions_stddev_fields)
    * [audit_logged_actions_stddev_pop_fields](#audit_logged_actions_stddev_pop_fields)
    * [audit_logged_actions_stddev_samp_fields](#audit_logged_actions_stddev_samp_fields)
    * [audit_logged_actions_sum_fields](#audit_logged_actions_sum_fields)
    * [audit_logged_actions_var_pop_fields](#audit_logged_actions_var_pop_fields)
    * [audit_logged_actions_var_samp_fields](#audit_logged_actions_var_samp_fields)
    * [audit_logged_actions_variance_fields](#audit_logged_actions_variance_fields)
    * [conceptnet_data](#conceptnet_data)
    * [conceptnet_data_aggregate](#conceptnet_data_aggregate)
    * [conceptnet_data_aggregate_fields](#conceptnet_data_aggregate_fields)
    * [conceptnet_data_avg_fields](#conceptnet_data_avg_fields)
    * [conceptnet_data_max_fields](#conceptnet_data_max_fields)
    * [conceptnet_data_min_fields](#conceptnet_data_min_fields)
    * [conceptnet_data_mutation_response](#conceptnet_data_mutation_response)
    * [conceptnet_data_stddev_fields](#conceptnet_data_stddev_fields)
    * [conceptnet_data_stddev_pop_fields](#conceptnet_data_stddev_pop_fields)
    * [conceptnet_data_stddev_samp_fields](#conceptnet_data_stddev_samp_fields)
    * [conceptnet_data_sum_fields](#conceptnet_data_sum_fields)
    * [conceptnet_data_var_pop_fields](#conceptnet_data_var_pop_fields)
    * [conceptnet_data_var_samp_fields](#conceptnet_data_var_samp_fields)
    * [conceptnet_data_variance_fields](#conceptnet_data_variance_fields)
    * [conversations](#conversations)
    * [conversations_aggregate](#conversations_aggregate)
    * [conversations_aggregate_fields](#conversations_aggregate_fields)
    * [conversations_avg_fields](#conversations_avg_fields)
    * [conversations_max_fields](#conversations_max_fields)
    * [conversations_min_fields](#conversations_min_fields)
    * [conversations_mutation_response](#conversations_mutation_response)
    * [conversations_stddev_fields](#conversations_stddev_fields)
    * [conversations_stddev_pop_fields](#conversations_stddev_pop_fields)
    * [conversations_stddev_samp_fields](#conversations_stddev_samp_fields)
    * [conversations_sum_fields](#conversations_sum_fields)
    * [conversations_var_pop_fields](#conversations_var_pop_fields)
    * [conversations_var_samp_fields](#conversations_var_samp_fields)
    * [conversations_variance_fields](#conversations_variance_fields)
    * [developers](#developers)
    * [developers_aggregate](#developers_aggregate)
    * [developers_aggregate_fields](#developers_aggregate_fields)
    * [developers_avg_fields](#developers_avg_fields)
    * [developers_max_fields](#developers_max_fields)
    * [developers_min_fields](#developers_min_fields)
    * [developers_mutation_response](#developers_mutation_response)
    * [developers_stddev_fields](#developers_stddev_fields)
    * [developers_stddev_pop_fields](#developers_stddev_pop_fields)
    * [developers_stddev_samp_fields](#developers_stddev_samp_fields)
    * [developers_sum_fields](#developers_sum_fields)
    * [developers_var_pop_fields](#developers_var_pop_fields)
    * [developers_var_samp_fields](#developers_var_samp_fields)
    * [developers_variance_fields](#developers_variance_fields)
    * [end_user_conversations](#end_user_conversations)
    * [end_user_conversations_aggregate](#end_user_conversations_aggregate)
    * [end_user_conversations_aggregate_fields](#end_user_conversations_aggregate_fields)
    * [end_user_conversations_avg_fields](#end_user_conversations_avg_fields)
    * [end_user_conversations_max_fields](#end_user_conversations_max_fields)
    * [end_user_conversations_min_fields](#end_user_conversations_min_fields)
    * [end_user_conversations_mutation_response](#end_user_conversations_mutation_response)
    * [end_user_conversations_stddev_fields](#end_user_conversations_stddev_fields)
    * [end_user_conversations_stddev_pop_fields](#end_user_conversations_stddev_pop_fields)
    * [end_user_conversations_stddev_samp_fields](#end_user_conversations_stddev_samp_fields)
    * [end_user_conversations_sum_fields](#end_user_conversations_sum_fields)
    * [end_user_conversations_var_pop_fields](#end_user_conversations_var_pop_fields)
    * [end_user_conversations_var_samp_fields](#end_user_conversations_var_samp_fields)
    * [end_user_conversations_variance_fields](#end_user_conversations_variance_fields)
    * [end_users](#end_users)
    * [end_users_aggregate](#end_users_aggregate)
    * [end_users_aggregate_fields](#end_users_aggregate_fields)
    * [end_users_avg_fields](#end_users_avg_fields)
    * [end_users_max_fields](#end_users_max_fields)
    * [end_users_min_fields](#end_users_min_fields)
    * [end_users_mutation_response](#end_users_mutation_response)
    * [end_users_stddev_fields](#end_users_stddev_fields)
    * [end_users_stddev_pop_fields](#end_users_stddev_pop_fields)
    * [end_users_stddev_samp_fields](#end_users_stddev_samp_fields)
    * [end_users_sum_fields](#end_users_sum_fields)
    * [end_users_var_pop_fields](#end_users_var_pop_fields)
    * [end_users_var_samp_fields](#end_users_var_samp_fields)
    * [end_users_variance_fields](#end_users_variance_fields)
    * [events](#events)
    * [events_aggregate](#events_aggregate)
    * [events_aggregate_fields](#events_aggregate_fields)
    * [events_max_fields](#events_max_fields)
    * [events_min_fields](#events_min_fields)
    * [events_mutation_response](#events_mutation_response)
    * [history](#history)
    * [history_aggregate](#history_aggregate)
    * [history_aggregate_fields](#history_aggregate_fields)
    * [history_avg_fields](#history_avg_fields)
    * [history_max_fields](#history_max_fields)
    * [history_min_fields](#history_min_fields)
    * [history_stddev_fields](#history_stddev_fields)
    * [history_stddev_pop_fields](#history_stddev_pop_fields)
    * [history_stddev_samp_fields](#history_stddev_samp_fields)
    * [history_sum_fields](#history_sum_fields)
    * [history_var_pop_fields](#history_var_pop_fields)
    * [history_var_samp_fields](#history_var_samp_fields)
    * [history_variance_fields](#history_variance_fields)
    * [kv_scope_enum](#kv_scope_enum)
    * [kv_scope_enum_aggregate](#kv_scope_enum_aggregate)
    * [kv_scope_enum_aggregate_fields](#kv_scope_enum_aggregate_fields)
    * [kv_scope_enum_max_fields](#kv_scope_enum_max_fields)
    * [kv_scope_enum_min_fields](#kv_scope_enum_min_fields)
    * [kv_scope_enum_mutation_response](#kv_scope_enum_mutation_response)
    * [kv_store](#kv_store)
    * [kv_store_aggregate](#kv_store_aggregate)
    * [kv_store_aggregate_fields](#kv_store_aggregate_fields)
    * [kv_store_avg_fields](#kv_store_avg_fields)
    * [kv_store_max_fields](#kv_store_max_fields)
    * [kv_store_min_fields](#kv_store_min_fields)
    * [kv_store_mutation_response](#kv_store_mutation_response)
    * [kv_store_stddev_fields](#kv_store_stddev_fields)
    * [kv_store_stddev_pop_fields](#kv_store_stddev_pop_fields)
    * [kv_store_stddev_samp_fields](#kv_store_stddev_samp_fields)
    * [kv_store_sum_fields](#kv_store_sum_fields)
    * [kv_store_var_pop_fields](#kv_store_var_pop_fields)
    * [kv_store_var_samp_fields](#kv_store_var_samp_fields)
    * [kv_store_variance_fields](#kv_store_variance_fields)
    * [last_utterance](#last_utterance)
    * [last_utterance_aggregate](#last_utterance_aggregate)
    * [last_utterance_aggregate_fields](#last_utterance_aggregate_fields)
    * [last_utterance_avg_fields](#last_utterance_avg_fields)
    * [last_utterance_max_fields](#last_utterance_max_fields)
    * [last_utterance_min_fields](#last_utterance_min_fields)
    * [last_utterance_stddev_fields](#last_utterance_stddev_fields)
    * [last_utterance_stddev_pop_fields](#last_utterance_stddev_pop_fields)
    * [last_utterance_stddev_samp_fields](#last_utterance_stddev_samp_fields)
    * [last_utterance_sum_fields](#last_utterance_sum_fields)
    * [last_utterance_var_pop_fields](#last_utterance_var_pop_fields)
    * [last_utterance_var_samp_fields](#last_utterance_var_samp_fields)
    * [last_utterance_variance_fields](#last_utterance_variance_fields)
    * [objects](#objects)
    * [objects_aggregate](#objects_aggregate)
    * [objects_aggregate_fields](#objects_aggregate_fields)
    * [objects_avg_fields](#objects_avg_fields)
    * [objects_max_fields](#objects_max_fields)
    * [objects_min_fields](#objects_min_fields)
    * [objects_mutation_response](#objects_mutation_response)
    * [objects_stddev_fields](#objects_stddev_fields)
    * [objects_stddev_pop_fields](#objects_stddev_pop_fields)
    * [objects_stddev_samp_fields](#objects_stddev_samp_fields)
    * [objects_sum_fields](#objects_sum_fields)
    * [objects_var_pop_fields](#objects_var_pop_fields)
    * [objects_var_samp_fields](#objects_var_samp_fields)
    * [objects_variance_fields](#objects_variance_fields)
    * [speaker_type_enum](#speaker_type_enum)
    * [speaker_type_enum_aggregate](#speaker_type_enum_aggregate)
    * [speaker_type_enum_aggregate_fields](#speaker_type_enum_aggregate_fields)
    * [speaker_type_enum_max_fields](#speaker_type_enum_max_fields)
    * [speaker_type_enum_min_fields](#speaker_type_enum_min_fields)
    * [speaker_type_enum_mutation_response](#speaker_type_enum_mutation_response)
    * [subscription_root](#subscription_root)
    * [utterances](#utterances)
    * [utterances_aggregate](#utterances_aggregate)
    * [utterances_aggregate_fields](#utterances_aggregate_fields)
    * [utterances_avg_fields](#utterances_avg_fields)
    * [utterances_max_fields](#utterances_max_fields)
    * [utterances_min_fields](#utterances_min_fields)
    * [utterances_mutation_response](#utterances_mutation_response)
    * [utterances_stddev_fields](#utterances_stddev_fields)
    * [utterances_stddev_pop_fields](#utterances_stddev_pop_fields)
    * [utterances_stddev_samp_fields](#utterances_stddev_samp_fields)
    * [utterances_sum_fields](#utterances_sum_fields)
    * [utterances_var_pop_fields](#utterances_var_pop_fields)
    * [utterances_var_samp_fields](#utterances_var_samp_fields)
    * [utterances_variance_fields](#utterances_variance_fields)
  * [Inputs](#inputs)
    * [Boolean_comparison_exp](#boolean_comparison_exp)
    * [ContextObject](#contextobject)
    * [InputPipe](#inputpipe)
    * [Int_comparison_exp](#int_comparison_exp)
    * [STTConfig](#sttconfig)
    * [String_comparison_exp](#string_comparison_exp)
    * [TTSConfig](#ttsconfig)
    * [Turn](#turn)
    * [_text_comparison_exp](#_text_comparison_exp)
    * [app_status_comparison_exp](#app_status_comparison_exp)
    * [apps_aggregate_order_by](#apps_aggregate_order_by)
    * [apps_append_input](#apps_append_input)
    * [apps_arr_rel_insert_input](#apps_arr_rel_insert_input)
    * [apps_avg_order_by](#apps_avg_order_by)
    * [apps_bool_exp](#apps_bool_exp)
    * [apps_delete_at_path_input](#apps_delete_at_path_input)
    * [apps_delete_elem_input](#apps_delete_elem_input)
    * [apps_delete_key_input](#apps_delete_key_input)
    * [apps_inc_input](#apps_inc_input)
    * [apps_insert_input](#apps_insert_input)
    * [apps_max_order_by](#apps_max_order_by)
    * [apps_min_order_by](#apps_min_order_by)
    * [apps_obj_rel_insert_input](#apps_obj_rel_insert_input)
    * [apps_on_conflict](#apps_on_conflict)
    * [apps_order_by](#apps_order_by)
    * [apps_prepend_input](#apps_prepend_input)
    * [apps_set_input](#apps_set_input)
    * [apps_stddev_order_by](#apps_stddev_order_by)
    * [apps_stddev_pop_order_by](#apps_stddev_pop_order_by)
    * [apps_stddev_samp_order_by](#apps_stddev_samp_order_by)
    * [apps_sum_order_by](#apps_sum_order_by)
    * [apps_var_pop_order_by](#apps_var_pop_order_by)
    * [apps_var_samp_order_by](#apps_var_samp_order_by)
    * [apps_variance_order_by](#apps_variance_order_by)
    * [atomic_data_bool_exp](#atomic_data_bool_exp)
    * [atomic_data_insert_input](#atomic_data_insert_input)
    * [atomic_data_order_by](#atomic_data_order_by)
    * [atomic_data_set_input](#atomic_data_set_input)
    * [audit_logged_actions_append_input](#audit_logged_actions_append_input)
    * [audit_logged_actions_bool_exp](#audit_logged_actions_bool_exp)
    * [audit_logged_actions_delete_at_path_input](#audit_logged_actions_delete_at_path_input)
    * [audit_logged_actions_delete_elem_input](#audit_logged_actions_delete_elem_input)
    * [audit_logged_actions_delete_key_input](#audit_logged_actions_delete_key_input)
    * [audit_logged_actions_inc_input](#audit_logged_actions_inc_input)
    * [audit_logged_actions_insert_input](#audit_logged_actions_insert_input)
    * [audit_logged_actions_on_conflict](#audit_logged_actions_on_conflict)
    * [audit_logged_actions_order_by](#audit_logged_actions_order_by)
    * [audit_logged_actions_pk_columns_input](#audit_logged_actions_pk_columns_input)
    * [audit_logged_actions_prepend_input](#audit_logged_actions_prepend_input)
    * [audit_logged_actions_set_input](#audit_logged_actions_set_input)
    * [bigint_comparison_exp](#bigint_comparison_exp)
    * [conceptnet_data_bool_exp](#conceptnet_data_bool_exp)
    * [conceptnet_data_inc_input](#conceptnet_data_inc_input)
    * [conceptnet_data_insert_input](#conceptnet_data_insert_input)
    * [conceptnet_data_on_conflict](#conceptnet_data_on_conflict)
    * [conceptnet_data_order_by](#conceptnet_data_order_by)
    * [conceptnet_data_set_input](#conceptnet_data_set_input)
    * [conceptnet_search_relations_args](#conceptnet_search_relations_args)
    * [conversations_aggregate_order_by](#conversations_aggregate_order_by)
    * [conversations_append_input](#conversations_append_input)
    * [conversations_arr_rel_insert_input](#conversations_arr_rel_insert_input)
    * [conversations_avg_order_by](#conversations_avg_order_by)
    * [conversations_bool_exp](#conversations_bool_exp)
    * [conversations_delete_at_path_input](#conversations_delete_at_path_input)
    * [conversations_delete_elem_input](#conversations_delete_elem_input)
    * [conversations_delete_key_input](#conversations_delete_key_input)
    * [conversations_inc_input](#conversations_inc_input)
    * [conversations_insert_input](#conversations_insert_input)
    * [conversations_max_order_by](#conversations_max_order_by)
    * [conversations_min_order_by](#conversations_min_order_by)
    * [conversations_obj_rel_insert_input](#conversations_obj_rel_insert_input)
    * [conversations_on_conflict](#conversations_on_conflict)
    * [conversations_order_by](#conversations_order_by)
    * [conversations_prepend_input](#conversations_prepend_input)
    * [conversations_set_input](#conversations_set_input)
    * [conversations_stddev_order_by](#conversations_stddev_order_by)
    * [conversations_stddev_pop_order_by](#conversations_stddev_pop_order_by)
    * [conversations_stddev_samp_order_by](#conversations_stddev_samp_order_by)
    * [conversations_sum_order_by](#conversations_sum_order_by)
    * [conversations_var_pop_order_by](#conversations_var_pop_order_by)
    * [conversations_var_samp_order_by](#conversations_var_samp_order_by)
    * [conversations_variance_order_by](#conversations_variance_order_by)
    * [developers_append_input](#developers_append_input)
    * [developers_bool_exp](#developers_bool_exp)
    * [developers_delete_at_path_input](#developers_delete_at_path_input)
    * [developers_delete_elem_input](#developers_delete_elem_input)
    * [developers_delete_key_input](#developers_delete_key_input)
    * [developers_inc_input](#developers_inc_input)
    * [developers_insert_input](#developers_insert_input)
    * [developers_obj_rel_insert_input](#developers_obj_rel_insert_input)
    * [developers_on_conflict](#developers_on_conflict)
    * [developers_order_by](#developers_order_by)
    * [developers_prepend_input](#developers_prepend_input)
    * [developers_set_input](#developers_set_input)
    * [end_user_conversations_aggregate_order_by](#end_user_conversations_aggregate_order_by)
    * [end_user_conversations_arr_rel_insert_input](#end_user_conversations_arr_rel_insert_input)
    * [end_user_conversations_avg_order_by](#end_user_conversations_avg_order_by)
    * [end_user_conversations_bool_exp](#end_user_conversations_bool_exp)
    * [end_user_conversations_inc_input](#end_user_conversations_inc_input)
    * [end_user_conversations_insert_input](#end_user_conversations_insert_input)
    * [end_user_conversations_max_order_by](#end_user_conversations_max_order_by)
    * [end_user_conversations_min_order_by](#end_user_conversations_min_order_by)
    * [end_user_conversations_on_conflict](#end_user_conversations_on_conflict)
    * [end_user_conversations_order_by](#end_user_conversations_order_by)
    * [end_user_conversations_pk_columns_input](#end_user_conversations_pk_columns_input)
    * [end_user_conversations_set_input](#end_user_conversations_set_input)
    * [end_user_conversations_stddev_order_by](#end_user_conversations_stddev_order_by)
    * [end_user_conversations_stddev_pop_order_by](#end_user_conversations_stddev_pop_order_by)
    * [end_user_conversations_stddev_samp_order_by](#end_user_conversations_stddev_samp_order_by)
    * [end_user_conversations_sum_order_by](#end_user_conversations_sum_order_by)
    * [end_user_conversations_var_pop_order_by](#end_user_conversations_var_pop_order_by)
    * [end_user_conversations_var_samp_order_by](#end_user_conversations_var_samp_order_by)
    * [end_user_conversations_variance_order_by](#end_user_conversations_variance_order_by)
    * [end_users_append_input](#end_users_append_input)
    * [end_users_bool_exp](#end_users_bool_exp)
    * [end_users_delete_at_path_input](#end_users_delete_at_path_input)
    * [end_users_delete_elem_input](#end_users_delete_elem_input)
    * [end_users_delete_key_input](#end_users_delete_key_input)
    * [end_users_inc_input](#end_users_inc_input)
    * [end_users_insert_input](#end_users_insert_input)
    * [end_users_obj_rel_insert_input](#end_users_obj_rel_insert_input)
    * [end_users_on_conflict](#end_users_on_conflict)
    * [end_users_order_by](#end_users_order_by)
    * [end_users_prepend_input](#end_users_prepend_input)
    * [end_users_set_input](#end_users_set_input)
    * [events_aggregate_order_by](#events_aggregate_order_by)
    * [events_append_input](#events_append_input)
    * [events_arr_rel_insert_input](#events_arr_rel_insert_input)
    * [events_bool_exp](#events_bool_exp)
    * [events_delete_at_path_input](#events_delete_at_path_input)
    * [events_delete_elem_input](#events_delete_elem_input)
    * [events_delete_key_input](#events_delete_key_input)
    * [events_insert_input](#events_insert_input)
    * [events_max_order_by](#events_max_order_by)
    * [events_min_order_by](#events_min_order_by)
    * [events_order_by](#events_order_by)
    * [events_prepend_input](#events_prepend_input)
    * [events_set_input](#events_set_input)
    * [history_bool_exp](#history_bool_exp)
    * [history_order_by](#history_order_by)
    * [inet_comparison_exp](#inet_comparison_exp)
    * [jsonb_comparison_exp](#jsonb_comparison_exp)
    * [kv_scope_enum_bool_exp](#kv_scope_enum_bool_exp)
    * [kv_scope_enum_insert_input](#kv_scope_enum_insert_input)
    * [kv_scope_enum_on_conflict](#kv_scope_enum_on_conflict)
    * [kv_scope_enum_order_by](#kv_scope_enum_order_by)
    * [kv_scope_enum_pk_columns_input](#kv_scope_enum_pk_columns_input)
    * [kv_scope_enum_set_input](#kv_scope_enum_set_input)
    * [kv_store_aggregate_order_by](#kv_store_aggregate_order_by)
    * [kv_store_append_input](#kv_store_append_input)
    * [kv_store_arr_rel_insert_input](#kv_store_arr_rel_insert_input)
    * [kv_store_avg_order_by](#kv_store_avg_order_by)
    * [kv_store_bool_exp](#kv_store_bool_exp)
    * [kv_store_delete_at_path_input](#kv_store_delete_at_path_input)
    * [kv_store_delete_elem_input](#kv_store_delete_elem_input)
    * [kv_store_delete_key_input](#kv_store_delete_key_input)
    * [kv_store_inc_input](#kv_store_inc_input)
    * [kv_store_insert_input](#kv_store_insert_input)
    * [kv_store_max_order_by](#kv_store_max_order_by)
    * [kv_store_min_order_by](#kv_store_min_order_by)
    * [kv_store_on_conflict](#kv_store_on_conflict)
    * [kv_store_order_by](#kv_store_order_by)
    * [kv_store_pk_columns_input](#kv_store_pk_columns_input)
    * [kv_store_prepend_input](#kv_store_prepend_input)
    * [kv_store_set_input](#kv_store_set_input)
    * [kv_store_stddev_order_by](#kv_store_stddev_order_by)
    * [kv_store_stddev_pop_order_by](#kv_store_stddev_pop_order_by)
    * [kv_store_stddev_samp_order_by](#kv_store_stddev_samp_order_by)
    * [kv_store_sum_order_by](#kv_store_sum_order_by)
    * [kv_store_var_pop_order_by](#kv_store_var_pop_order_by)
    * [kv_store_var_samp_order_by](#kv_store_var_samp_order_by)
    * [kv_store_variance_order_by](#kv_store_variance_order_by)
    * [last_utterance_bool_exp](#last_utterance_bool_exp)
    * [last_utterance_order_by](#last_utterance_order_by)
    * [numeric_comparison_exp](#numeric_comparison_exp)
    * [objects_append_input](#objects_append_input)
    * [objects_bool_exp](#objects_bool_exp)
    * [objects_delete_at_path_input](#objects_delete_at_path_input)
    * [objects_delete_elem_input](#objects_delete_elem_input)
    * [objects_delete_key_input](#objects_delete_key_input)
    * [objects_inc_input](#objects_inc_input)
    * [objects_insert_input](#objects_insert_input)
    * [objects_on_conflict](#objects_on_conflict)
    * [objects_order_by](#objects_order_by)
    * [objects_pk_columns_input](#objects_pk_columns_input)
    * [objects_prepend_input](#objects_prepend_input)
    * [objects_set_input](#objects_set_input)
    * [oid_comparison_exp](#oid_comparison_exp)
    * [speaker_type_enum_bool_exp](#speaker_type_enum_bool_exp)
    * [speaker_type_enum_enum_comparison_exp](#speaker_type_enum_enum_comparison_exp)
    * [speaker_type_enum_insert_input](#speaker_type_enum_insert_input)
    * [speaker_type_enum_obj_rel_insert_input](#speaker_type_enum_obj_rel_insert_input)
    * [speaker_type_enum_on_conflict](#speaker_type_enum_on_conflict)
    * [speaker_type_enum_order_by](#speaker_type_enum_order_by)
    * [speaker_type_enum_pk_columns_input](#speaker_type_enum_pk_columns_input)
    * [speaker_type_enum_set_input](#speaker_type_enum_set_input)
    * [timestamptz_comparison_exp](#timestamptz_comparison_exp)
    * [tstzrange_comparison_exp](#tstzrange_comparison_exp)
    * [utterances_aggregate_order_by](#utterances_aggregate_order_by)
    * [utterances_arr_rel_insert_input](#utterances_arr_rel_insert_input)
    * [utterances_avg_order_by](#utterances_avg_order_by)
    * [utterances_bool_exp](#utterances_bool_exp)
    * [utterances_inc_input](#utterances_inc_input)
    * [utterances_insert_input](#utterances_insert_input)
    * [utterances_max_order_by](#utterances_max_order_by)
    * [utterances_min_order_by](#utterances_min_order_by)
    * [utterances_order_by](#utterances_order_by)
    * [utterances_set_input](#utterances_set_input)
    * [utterances_stddev_order_by](#utterances_stddev_order_by)
    * [utterances_stddev_pop_order_by](#utterances_stddev_pop_order_by)
    * [utterances_stddev_samp_order_by](#utterances_stddev_samp_order_by)
    * [utterances_sum_order_by](#utterances_sum_order_by)
    * [utterances_var_pop_order_by](#utterances_var_pop_order_by)
    * [utterances_var_samp_order_by](#utterances_var_samp_order_by)
    * [utterances_variance_order_by](#utterances_variance_order_by)
  * [Enums](#enums)
    * [ACEOutputType](#aceoutputtype)
    * [Agent](#agent)
    * [AudioEncoding](#audioencoding)
    * [Category](#category)
    * [Encoding](#encoding)
    * [Relation](#relation)
    * [ServiceName](#servicename)
    * [apps_constraint](#apps_constraint)
    * [apps_select_column](#apps_select_column)
    * [apps_update_column](#apps_update_column)
    * [atomic_data_select_column](#atomic_data_select_column)
    * [audit_logged_actions_constraint](#audit_logged_actions_constraint)
    * [audit_logged_actions_select_column](#audit_logged_actions_select_column)
    * [audit_logged_actions_update_column](#audit_logged_actions_update_column)
    * [conceptnet_data_constraint](#conceptnet_data_constraint)
    * [conceptnet_data_select_column](#conceptnet_data_select_column)
    * [conceptnet_data_update_column](#conceptnet_data_update_column)
    * [conversations_constraint](#conversations_constraint)
    * [conversations_select_column](#conversations_select_column)
    * [conversations_update_column](#conversations_update_column)
    * [developers_constraint](#developers_constraint)
    * [developers_select_column](#developers_select_column)
    * [developers_update_column](#developers_update_column)
    * [end_user_conversations_constraint](#end_user_conversations_constraint)
    * [end_user_conversations_select_column](#end_user_conversations_select_column)
    * [end_user_conversations_update_column](#end_user_conversations_update_column)
    * [end_users_constraint](#end_users_constraint)
    * [end_users_select_column](#end_users_select_column)
    * [end_users_update_column](#end_users_update_column)
    * [events_select_column](#events_select_column)
    * [history_select_column](#history_select_column)
    * [kv_scope_enum_constraint](#kv_scope_enum_constraint)
    * [kv_scope_enum_select_column](#kv_scope_enum_select_column)
    * [kv_scope_enum_update_column](#kv_scope_enum_update_column)
    * [kv_store_constraint](#kv_store_constraint)
    * [kv_store_select_column](#kv_store_select_column)
    * [kv_store_update_column](#kv_store_update_column)
    * [last_utterance_select_column](#last_utterance_select_column)
    * [objects_constraint](#objects_constraint)
    * [objects_select_column](#objects_select_column)
    * [objects_update_column](#objects_update_column)
    * [order_by](#order_by)
    * [speaker_type_enum_constraint](#speaker_type_enum_constraint)
    * [speaker_type_enum_enum](#speaker_type_enum_enum)
    * [speaker_type_enum_select_column](#speaker_type_enum_select_column)
    * [speaker_type_enum_update_column](#speaker_type_enum_update_column)
    * [utterances_select_column](#utterances_select_column)
  * [Scalars](#scalars)
    * [Boolean](#boolean)
    * [Float](#float)
    * [Int](#int)
    * [JSON](#json)
    * [String](#string)
    * [_text](#_text)
    * [app_status](#app_status)
    * [bigint](#bigint)
    * [inet](#inet)
    * [jsonb](#jsonb)
    * [numeric](#numeric)
    * [oid](#oid)
    * [timestamptz](#timestamptz)
    * [tstzrange](#tstzrange)
  * [Interfaces](#interfaces)
    * [Container](#container)

</details>

## Query (query_root)
<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps_aggregate</strong></td>
<td valign="top"><a href="#apps_aggregate">apps_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>atomic_data</strong></td>
<td valign="top">[<a href="#atomic_data">atomic_data</a>!]!</td>
<td>

fetch data from the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#atomic_data_select_column">atomic_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#atomic_data_order_by">atomic_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>atomic_data_aggregate</strong></td>
<td valign="top"><a href="#atomic_data_aggregate">atomic_data_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#atomic_data_select_column">atomic_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#atomic_data_order_by">atomic_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions</strong></td>
<td valign="top">[<a href="#audit_logged_actions">audit_logged_actions</a>!]!</td>
<td>

fetch data from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#audit_logged_actions_select_column">audit_logged_actions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#audit_logged_actions_order_by">audit_logged_actions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions_aggregate</strong></td>
<td valign="top"><a href="#audit_logged_actions_aggregate">audit_logged_actions_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#audit_logged_actions_select_column">audit_logged_actions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#audit_logged_actions_order_by">audit_logged_actions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions_by_pk</strong></td>
<td valign="top"><a href="#audit_logged_actions">audit_logged_actions</a></td>
<td>

fetch data from the table: "audit.logged_actions" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">action_tstamp_stm</td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">event_id</td>
<td valign="top"><a href="#bigint">bigint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callApplyVoiceCSS</strong></td>
<td valign="top"><a href="#ssmlresult">SSMLResult</a></td>
<td>

Apply voice CSS to the SSML input

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">styled_ssml</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">voice_css</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callChitchat</strong></td>
<td valign="top"><a href="#chitchatresponse">ChitchatResponse</a></td>
<td>

Perform chit chat

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">history</td>
<td valign="top">[<a href="#turn">Turn</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callClassifyTopic</strong></td>
<td valign="top"><a href="#classificationresult">ClassificationResult</a></td>
<td>

Classify topics

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">allow_multiple</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Allow multiple topics to be applicable

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">topics</td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callCommonsense</strong></td>
<td valign="top"><a href="#relationresult">RelationResult</a></td>
<td>

Predict category

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">category</td>
<td valign="top"><a href="#category">Category</a></td>
<td>

Category to extract from input

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text string

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callCompose</strong></td>
<td valign="top"><a href="#composeresult">ComposeResult</a></td>
<td>

Execute composition pipeline

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">init</td>
<td valign="top"><a href="#json">JSON</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pipeline</td>
<td valign="top">[<a href="#inputpipe">InputPipe</a>]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callMatchIntent</strong></td>
<td valign="top"><a href="#matchintentoutput">MatchIntentOutput</a></td>
<td>

Call the intent matching functionality

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">possible_intents</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">similarity_threshold</td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callMeasureSimilarity</strong></td>
<td valign="top"><a href="#sentencesimilarityscores">SentenceSimilarityScores</a></td>
<td>

Measure sentences similarity

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">candidates</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callNLU</strong></td>
<td valign="top"><a href="#nluresult">NLUResult</a></td>
<td>

Document processing

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text to perform NLU tasks on

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callNextDialogTurn</strong></td>
<td valign="top"><a href="#result">Result</a></td>
<td>

Perform next dialog turn prediction

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">history</td>
<td valign="top">[<a href="#turn">Turn</a>!]</td>
<td>

Utterances history

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Alternatives to choose from

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callParaphraseSentence</strong></td>
<td valign="top"><a href="#paraphrase">Paraphrase</a></td>
<td>

Perform sentence paraphrasing

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callParseACE</strong></td>
<td valign="top"><a href="#aceresult">ACEResult</a></td>
<td>

Parse ACE sentence

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">format</td>
<td valign="top"><a href="#aceoutputtype">ACEOutputType</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">guess</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callParseContext</strong></td>
<td valign="top">[<a href="#contextresult">ContextResult</a>]</td>
<td>

Parse frame semantics for a list of dialog turns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">turns</td>
<td valign="top">[<a href="#contextobject">ContextObject</a>]</td>
<td>

List of possible turns

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callPredictRelation</strong></td>
<td valign="top"><a href="#relationresult">RelationResult</a></td>
<td>

Predict relations

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text string

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">relation</td>
<td valign="top"><a href="#relation">Relation</a></td>
<td>

Relation to extract from input

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callQA</strong></td>
<td valign="top"><a href="#qa_result">QA_Result</a></td>
<td>

Answer questions based on context

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">choices</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Alternatives to choose answer from

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">context</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">min_length</td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callResolveCoreference</strong></td>
<td valign="top"><a href="#corefresult">CorefResult</a></td>
<td>

Coreference resolution

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text to perform coreference resolution on

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callSentimentAnalysis</strong></td>
<td valign="top">[<a href="#sentimentanalysisresult">SentimentAnalysisResult</a>]</td>
<td>

Sentiment analisys

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text to perform sentiment analysis on

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callShowDocs</strong></td>
<td valign="top"><a href="#serviceinfo">ServiceInfo</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">service</td>
<td valign="top"><a href="#servicename">ServiceName</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callSpeechToText</strong></td>
<td valign="top">[<a href="#sttresult">STTResult</a>]</td>
<td>

Convert speech to text

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">audioB64</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">config</td>
<td valign="top"><a href="#sttconfig">STTConfig</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>callTextToSpeech</strong></td>
<td valign="top"><a href="#ttsresult">TTSResult</a></td>
<td>

Convert text to speech

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">config</td>
<td valign="top"><a href="#ttsconfig">TTSConfig</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">text</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_data</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td>

fetch data from the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_data_aggregate</strong></td>
<td valign="top"><a href="#conceptnet_data_aggregate">conceptnet_data_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_search_relations</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td>

execute function "conceptnet.search_relations" which returns "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">args</td>
<td valign="top"><a href="#conceptnet_search_relations_args">conceptnet_search_relations_args</a>!</td>
<td>

input parameters for function "conceptnet.search_relations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_search_relations_aggregate</strong></td>
<td valign="top"><a href="#conceptnet_data_aggregate">conceptnet_data_aggregate</a>!</td>
<td>

execute function "conceptnet.search_relations" and query aggregates on result of table type "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">args</td>
<td valign="top"><a href="#conceptnet_search_relations_args">conceptnet_search_relations_args</a>!</td>
<td>

input parameters for function "conceptnet.search_relations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate">conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>deprecatedCallNlpDoc</strong></td>
<td valign="top"><a href="#nlpdoc">NlpDoc</a></td>
<td>

Document processing

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">disable</td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

List of pipes to disable

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">input</td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Text to perform process

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">model</td>
<td valign="top"><a href="#string">String</a></td>
<td>

Name of the spaCy model to use

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

fetch data from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers_aggregate</strong></td>
<td valign="top"><a href="#developers_aggregate">developers_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate">end_user_conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

fetch data from the table: "end_user_conversations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">conversation_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">end_user_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_users</strong></td>
<td valign="top">[<a href="#end_users">end_users</a>!]!</td>
<td>

fetch data from the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_users_select_column">end_users_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_users_order_by">end_users_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_users_aggregate</strong></td>
<td valign="top"><a href="#end_users_aggregate">end_users_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_users_select_column">end_users_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_users_order_by">end_users_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events</strong></td>
<td valign="top">[<a href="#events">events</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events_aggregate</strong></td>
<td valign="top"><a href="#events_aggregate">events_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history</strong></td>
<td valign="top">[<a href="#history">history</a>!]!</td>
<td>

fetch data from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history_aggregate</strong></td>
<td valign="top"><a href="#history_aggregate">history_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum</strong></td>
<td valign="top">[<a href="#kv_scope_enum">kv_scope_enum</a>!]!</td>
<td>

fetch data from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_scope_enum_select_column">kv_scope_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_scope_enum_order_by">kv_scope_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum_aggregate</strong></td>
<td valign="top"><a href="#kv_scope_enum_aggregate">kv_scope_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_scope_enum_select_column">kv_scope_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_scope_enum_order_by">kv_scope_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum_by_pk</strong></td>
<td valign="top"><a href="#kv_scope_enum">kv_scope_enum</a></td>
<td>

fetch data from the table: "kv_scope_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

fetch data from the table: "kv_store" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">key</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope_object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance</strong></td>
<td valign="top">[<a href="#last_utterance">last_utterance</a>!]!</td>
<td>

fetch data from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance_aggregate</strong></td>
<td valign="top"><a href="#last_utterance_aggregate">last_utterance_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>me</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

execute function "me" which returns "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>me_aggregate</strong></td>
<td valign="top"><a href="#developers_aggregate">developers_aggregate</a>!</td>
<td>

execute function "me" and query aggregates on result of table type "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects</strong></td>
<td valign="top">[<a href="#objects">objects</a>!]!</td>
<td>

fetch data from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#objects_select_column">objects_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#objects_order_by">objects_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects_aggregate</strong></td>
<td valign="top"><a href="#objects_aggregate">objects_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#objects_select_column">objects_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#objects_order_by">objects_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects_by_pk</strong></td>
<td valign="top"><a href="#objects">objects</a></td>
<td>

fetch data from the table: "objects" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top">[<a href="#speaker_type_enum">speaker_type_enum</a>!]!</td>
<td>

fetch data from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#speaker_type_enum_select_column">speaker_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#speaker_type_enum_order_by">speaker_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum_aggregate</strong></td>
<td valign="top"><a href="#speaker_type_enum_aggregate">speaker_type_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#speaker_type_enum_select_column">speaker_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#speaker_type_enum_order_by">speaker_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum_by_pk</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a></td>
<td>

fetch data from the table: "speaker_type_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate">utterances_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

## Mutation (mutation_root)
mutation root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>delete_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

delete data from the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_atomic_data</strong></td>
<td valign="top"><a href="#atomic_data_mutation_response">atomic_data_mutation_response</a></td>
<td>

delete data from the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_audit_logged_actions</strong></td>
<td valign="top"><a href="#audit_logged_actions_mutation_response">audit_logged_actions_mutation_response</a></td>
<td>

delete data from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_audit_logged_actions_by_pk</strong></td>
<td valign="top"><a href="#audit_logged_actions">audit_logged_actions</a></td>
<td>

delete single row from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">action_tstamp_stm</td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">event_id</td>
<td valign="top"><a href="#bigint">bigint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_conceptnet_data</strong></td>
<td valign="top"><a href="#conceptnet_data_mutation_response">conceptnet_data_mutation_response</a></td>
<td>

delete data from the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

delete data from the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_developers</strong></td>
<td valign="top"><a href="#developers_mutation_response">developers_mutation_response</a></td>
<td>

delete data from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_mutation_response">end_user_conversations_mutation_response</a></td>
<td>

delete data from the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

delete single row from the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">conversation_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">end_user_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_end_users</strong></td>
<td valign="top"><a href="#end_users_mutation_response">end_users_mutation_response</a></td>
<td>

delete data from the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_events</strong></td>
<td valign="top"><a href="#events_mutation_response">events_mutation_response</a></td>
<td>

delete data from the table: "events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_kv_scope_enum</strong></td>
<td valign="top"><a href="#kv_scope_enum_mutation_response">kv_scope_enum_mutation_response</a></td>
<td>

delete data from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_kv_scope_enum_by_pk</strong></td>
<td valign="top"><a href="#kv_scope_enum">kv_scope_enum</a></td>
<td>

delete single row from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_kv_store</strong></td>
<td valign="top"><a href="#kv_store_mutation_response">kv_store_mutation_response</a></td>
<td>

delete data from the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

delete single row from the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">key</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope_object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_objects</strong></td>
<td valign="top"><a href="#objects_mutation_response">objects_mutation_response</a></td>
<td>

delete data from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_objects_by_pk</strong></td>
<td valign="top"><a href="#objects">objects</a></td>
<td>

delete single row from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_mutation_response">speaker_type_enum_mutation_response</a></td>
<td>

delete data from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_speaker_type_enum_by_pk</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a></td>
<td>

delete single row from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>delete_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

delete data from the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a>!</td>
<td>

filter the rows which have to be deleted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

insert data into the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#apps_insert_input">apps_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_apps_one</strong></td>
<td valign="top"><a href="#apps">apps</a></td>
<td>

insert a single row into the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#apps_insert_input">apps_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_atomic_data</strong></td>
<td valign="top"><a href="#atomic_data_mutation_response">atomic_data_mutation_response</a></td>
<td>

insert data into the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#atomic_data_insert_input">atomic_data_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_atomic_data_one</strong></td>
<td valign="top"><a href="#atomic_data">atomic_data</a></td>
<td>

insert a single row into the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#atomic_data_insert_input">atomic_data_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_audit_logged_actions</strong></td>
<td valign="top"><a href="#audit_logged_actions_mutation_response">audit_logged_actions_mutation_response</a></td>
<td>

insert data into the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#audit_logged_actions_insert_input">audit_logged_actions_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#audit_logged_actions_on_conflict">audit_logged_actions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_audit_logged_actions_one</strong></td>
<td valign="top"><a href="#audit_logged_actions">audit_logged_actions</a></td>
<td>

insert a single row into the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#audit_logged_actions_insert_input">audit_logged_actions_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#audit_logged_actions_on_conflict">audit_logged_actions_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conceptnet_data</strong></td>
<td valign="top"><a href="#conceptnet_data_mutation_response">conceptnet_data_mutation_response</a></td>
<td>

insert data into the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#conceptnet_data_insert_input">conceptnet_data_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conceptnet_data_on_conflict">conceptnet_data_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conceptnet_data_one</strong></td>
<td valign="top"><a href="#conceptnet_data">conceptnet_data</a></td>
<td>

insert a single row into the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#conceptnet_data_insert_input">conceptnet_data_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conceptnet_data_on_conflict">conceptnet_data_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

insert data into the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#conversations_insert_input">conversations_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_conversations_one</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

insert a single row into the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#conversations_insert_input">conversations_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_developers</strong></td>
<td valign="top"><a href="#developers_mutation_response">developers_mutation_response</a></td>
<td>

insert data into the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#developers_insert_input">developers_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#developers_on_conflict">developers_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_developers_one</strong></td>
<td valign="top"><a href="#developers">developers</a></td>
<td>

insert a single row into the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#developers_insert_input">developers_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#developers_on_conflict">developers_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_mutation_response">end_user_conversations_mutation_response</a></td>
<td>

insert data into the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#end_user_conversations_on_conflict">end_user_conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_user_conversations_one</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

insert a single row into the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#end_user_conversations_on_conflict">end_user_conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_users</strong></td>
<td valign="top"><a href="#end_users_mutation_response">end_users_mutation_response</a></td>
<td>

insert data into the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#end_users_insert_input">end_users_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#end_users_on_conflict">end_users_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_end_users_one</strong></td>
<td valign="top"><a href="#end_users">end_users</a></td>
<td>

insert a single row into the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#end_users_insert_input">end_users_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#end_users_on_conflict">end_users_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_events</strong></td>
<td valign="top"><a href="#events_mutation_response">events_mutation_response</a></td>
<td>

insert data into the table: "events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#events_insert_input">events_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_events_one</strong></td>
<td valign="top"><a href="#events">events</a></td>
<td>

insert a single row into the table: "events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#events_insert_input">events_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_kv_scope_enum</strong></td>
<td valign="top"><a href="#kv_scope_enum_mutation_response">kv_scope_enum_mutation_response</a></td>
<td>

insert data into the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#kv_scope_enum_insert_input">kv_scope_enum_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#kv_scope_enum_on_conflict">kv_scope_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_kv_scope_enum_one</strong></td>
<td valign="top"><a href="#kv_scope_enum">kv_scope_enum</a></td>
<td>

insert a single row into the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#kv_scope_enum_insert_input">kv_scope_enum_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#kv_scope_enum_on_conflict">kv_scope_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_kv_store</strong></td>
<td valign="top"><a href="#kv_store_mutation_response">kv_store_mutation_response</a></td>
<td>

insert data into the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#kv_store_insert_input">kv_store_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#kv_store_on_conflict">kv_store_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_kv_store_one</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

insert a single row into the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#kv_store_insert_input">kv_store_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#kv_store_on_conflict">kv_store_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_objects</strong></td>
<td valign="top"><a href="#objects_mutation_response">objects_mutation_response</a></td>
<td>

insert data into the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#objects_insert_input">objects_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#objects_on_conflict">objects_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_objects_one</strong></td>
<td valign="top"><a href="#objects">objects</a></td>
<td>

insert a single row into the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#objects_insert_input">objects_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#objects_on_conflict">objects_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_mutation_response">speaker_type_enum_mutation_response</a></td>
<td>

insert data into the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#speaker_type_enum_insert_input">speaker_type_enum_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#speaker_type_enum_on_conflict">speaker_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_speaker_type_enum_one</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a></td>
<td>

insert a single row into the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#speaker_type_enum_insert_input">speaker_type_enum_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">on_conflict</td>
<td valign="top"><a href="#speaker_type_enum_on_conflict">speaker_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

insert data into the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">objects</td>
<td valign="top">[<a href="#utterances_insert_input">utterances_insert_input</a>!]!</td>
<td>

the rows to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>insert_utterances_one</strong></td>
<td valign="top"><a href="#utterances">utterances</a></td>
<td>

insert a single row into the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object</td>
<td valign="top"><a href="#utterances_insert_input">utterances_insert_input</a>!</td>
<td>

the row to be inserted

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_apps</strong></td>
<td valign="top"><a href="#apps_mutation_response">apps_mutation_response</a></td>
<td>

update data of the table: "apps"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#apps_append_input">apps_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#apps_delete_at_path_input">apps_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#apps_delete_elem_input">apps_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#apps_delete_key_input">apps_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#apps_inc_input">apps_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#apps_prepend_input">apps_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#apps_set_input">apps_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_atomic_data</strong></td>
<td valign="top"><a href="#atomic_data_mutation_response">atomic_data_mutation_response</a></td>
<td>

update data of the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#atomic_data_set_input">atomic_data_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_audit_logged_actions</strong></td>
<td valign="top"><a href="#audit_logged_actions_mutation_response">audit_logged_actions_mutation_response</a></td>
<td>

update data of the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#audit_logged_actions_append_input">audit_logged_actions_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#audit_logged_actions_delete_at_path_input">audit_logged_actions_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#audit_logged_actions_delete_elem_input">audit_logged_actions_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#audit_logged_actions_delete_key_input">audit_logged_actions_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#audit_logged_actions_inc_input">audit_logged_actions_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#audit_logged_actions_prepend_input">audit_logged_actions_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#audit_logged_actions_set_input">audit_logged_actions_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_audit_logged_actions_by_pk</strong></td>
<td valign="top"><a href="#audit_logged_actions">audit_logged_actions</a></td>
<td>

update single row of the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#audit_logged_actions_append_input">audit_logged_actions_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#audit_logged_actions_delete_at_path_input">audit_logged_actions_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#audit_logged_actions_delete_elem_input">audit_logged_actions_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#audit_logged_actions_delete_key_input">audit_logged_actions_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#audit_logged_actions_inc_input">audit_logged_actions_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#audit_logged_actions_prepend_input">audit_logged_actions_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#audit_logged_actions_set_input">audit_logged_actions_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#audit_logged_actions_pk_columns_input">audit_logged_actions_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_conceptnet_data</strong></td>
<td valign="top"><a href="#conceptnet_data_mutation_response">conceptnet_data_mutation_response</a></td>
<td>

update data of the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#conceptnet_data_inc_input">conceptnet_data_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#conceptnet_data_set_input">conceptnet_data_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_conversations</strong></td>
<td valign="top"><a href="#conversations_mutation_response">conversations_mutation_response</a></td>
<td>

update data of the table: "conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#conversations_append_input">conversations_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#conversations_delete_at_path_input">conversations_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#conversations_delete_elem_input">conversations_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#conversations_delete_key_input">conversations_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#conversations_inc_input">conversations_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#conversations_prepend_input">conversations_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#conversations_set_input">conversations_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_developers</strong></td>
<td valign="top"><a href="#developers_mutation_response">developers_mutation_response</a></td>
<td>

update data of the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#developers_append_input">developers_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#developers_delete_at_path_input">developers_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#developers_delete_elem_input">developers_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#developers_delete_key_input">developers_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#developers_inc_input">developers_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#developers_prepend_input">developers_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#developers_set_input">developers_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_mutation_response">end_user_conversations_mutation_response</a></td>
<td>

update data of the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#end_user_conversations_inc_input">end_user_conversations_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#end_user_conversations_set_input">end_user_conversations_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

update single row of the table: "end_user_conversations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#end_user_conversations_inc_input">end_user_conversations_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#end_user_conversations_set_input">end_user_conversations_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#end_user_conversations_pk_columns_input">end_user_conversations_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_end_users</strong></td>
<td valign="top"><a href="#end_users_mutation_response">end_users_mutation_response</a></td>
<td>

update data of the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#end_users_append_input">end_users_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#end_users_delete_at_path_input">end_users_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#end_users_delete_elem_input">end_users_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#end_users_delete_key_input">end_users_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#end_users_inc_input">end_users_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#end_users_prepend_input">end_users_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#end_users_set_input">end_users_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_events</strong></td>
<td valign="top"><a href="#events_mutation_response">events_mutation_response</a></td>
<td>

update data of the table: "events"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#events_append_input">events_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#events_delete_at_path_input">events_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#events_delete_elem_input">events_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#events_delete_key_input">events_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#events_prepend_input">events_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#events_set_input">events_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_kv_scope_enum</strong></td>
<td valign="top"><a href="#kv_scope_enum_mutation_response">kv_scope_enum_mutation_response</a></td>
<td>

update data of the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#kv_scope_enum_set_input">kv_scope_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_kv_scope_enum_by_pk</strong></td>
<td valign="top"><a href="#kv_scope_enum">kv_scope_enum</a></td>
<td>

update single row of the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#kv_scope_enum_set_input">kv_scope_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#kv_scope_enum_pk_columns_input">kv_scope_enum_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_kv_store</strong></td>
<td valign="top"><a href="#kv_store_mutation_response">kv_store_mutation_response</a></td>
<td>

update data of the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#kv_store_append_input">kv_store_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#kv_store_delete_at_path_input">kv_store_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#kv_store_delete_elem_input">kv_store_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#kv_store_delete_key_input">kv_store_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#kv_store_inc_input">kv_store_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#kv_store_prepend_input">kv_store_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#kv_store_set_input">kv_store_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

update single row of the table: "kv_store"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#kv_store_append_input">kv_store_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#kv_store_delete_at_path_input">kv_store_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#kv_store_delete_elem_input">kv_store_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#kv_store_delete_key_input">kv_store_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#kv_store_inc_input">kv_store_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#kv_store_prepend_input">kv_store_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#kv_store_set_input">kv_store_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#kv_store_pk_columns_input">kv_store_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_objects</strong></td>
<td valign="top"><a href="#objects_mutation_response">objects_mutation_response</a></td>
<td>

update data of the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#objects_append_input">objects_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#objects_delete_at_path_input">objects_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#objects_delete_elem_input">objects_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#objects_delete_key_input">objects_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#objects_inc_input">objects_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#objects_prepend_input">objects_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#objects_set_input">objects_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_objects_by_pk</strong></td>
<td valign="top"><a href="#objects">objects</a></td>
<td>

update single row of the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_append</td>
<td valign="top"><a href="#objects_append_input">objects_append_input</a></td>
<td>

append existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_at_path</td>
<td valign="top"><a href="#objects_delete_at_path_input">objects_delete_at_path_input</a></td>
<td>

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_elem</td>
<td valign="top"><a href="#objects_delete_elem_input">objects_delete_elem_input</a></td>
<td>

delete the array element with specified index (negative integers count from
the end). throws an error if top level container is not an array

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_delete_key</td>
<td valign="top"><a href="#objects_delete_key_input">objects_delete_key_input</a></td>
<td>

delete key/value pair or string element. key/value pairs are matched based on their key value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#objects_inc_input">objects_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_prepend</td>
<td valign="top"><a href="#objects_prepend_input">objects_prepend_input</a></td>
<td>

prepend existing jsonb value of filtered columns with new jsonb value

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#objects_set_input">objects_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#objects_pk_columns_input">objects_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_mutation_response">speaker_type_enum_mutation_response</a></td>
<td>

update data of the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#speaker_type_enum_set_input">speaker_type_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_speaker_type_enum_by_pk</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a></td>
<td>

update single row of the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#speaker_type_enum_set_input">speaker_type_enum_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">pk_columns</td>
<td valign="top"><a href="#speaker_type_enum_pk_columns_input">speaker_type_enum_pk_columns_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_utterances</strong></td>
<td valign="top"><a href="#utterances_mutation_response">utterances_mutation_response</a></td>
<td>

update data of the table: "utterances"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_inc</td>
<td valign="top"><a href="#utterances_inc_input">utterances_inc_input</a></td>
<td>

increments the numeric columns with given value of the filtered values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">_set</td>
<td valign="top"><a href="#utterances_set_input">utterances_set_input</a></td>
<td>

sets the columns of the filtered rows to the given values

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a>!</td>
<td>

filter the rows which have to be updated

</td>
</tr>
</tbody>
</table>

## Objects

### ACEResult

Output type

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

APE output

</td>
</tr>
</tbody>
</table>

### Cat

Category applied to whole document (label, score), or to spans (start, end, label, score).

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Span end position

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>label</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Document label

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Document score

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Span start position

</td>
</tr>
</tbody>
</table>

### ChitchatResponse

Chitchat results

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### ClassificationResult

Topic classification results

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#topicscore">TopicScore</a>]</td>
<td></td>
</tr>
</tbody>
</table>

### ComposeResult

Output result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Resulting JSON

</td>
</tr>
</tbody>
</table>

### ContextResult

SLING document container

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>context</strong></td>
<td valign="top"><a href="#slingdocument">SlingDocument</a></td>
<td>

SLING document

</td>
</tr>
</tbody>
</table>

### CorefCluster

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>i</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Index of the cluster in the Doc

</td>
</tr>
</tbody>
</table>

### CorefResult

Coreference resolution data

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coreferences</strong></td>
<td valign="top">[<a href="#corefresultscores">CorefResultScores</a>]</td>
<td>

Scores of the coreference resolution between mentions.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_coreference</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Has any coreference has been resolved in the Doc

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Unicode representation of the doc where each corefering mention is replaced by the main mention in the associated cluster.

</td>
</tr>
</tbody>
</table>

### CorefResultScores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mention</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cluster mention

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>reference</strong></td>
<td valign="top">[<a href="#resultscores">ResultScores</a>]</td>
<td>

Scores of the coreference resolution between mentions.

</td>
</tr>
</tbody>
</table>

### CorefScores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mention</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Cluster mention

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scores</strong></td>
<td valign="top">[<a href="#scores">Scores</a>]</td>
<td>

Scores of the coreference resolution between mentions.

</td>
</tr>
</tbody>
</table>

### DialogAlternative

One of the alternatives, among which the next turn must be chosen

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternative</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Content of the utterance

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Confidence of the utterance

</td>
</tr>
</tbody>
</table>

### DocExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coref_clusters</strong></td>
<td valign="top">[<a href="#corefcluster">CorefCluster</a>]</td>
<td>

All the clusters of corefering mentions in the doc

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coref_resolved</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Unicode representation of the doc where each corefering mention is replaced by the main mention in the associated cluster.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coref_scores</strong></td>
<td valign="top">[<a href="#corefscores">CorefScores</a>]</td>
<td>

Scores of the coreference resolution between mentions.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_coref</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Has any coreference has been resolved in the Doc

</td>
</tr>
</tbody>
</table>

### MatchIntentOutput

Intent matching output

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#phrasematch">PhraseMatch</a>]</td>
<td>

A list of matches found

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>warnings</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A list of processing errors if any

</td>
</tr>
</tbody>
</table>

### NLUResult

A container for accessing linguistic annotations. Access sentences and named entities.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>entities</strong></td>
<td valign="top">[<a href="#nluspan">NLUSpan</a>]</td>
<td>

The named entities in the document. Returns a list of named entity Span
objects, if the entity recognizer has been applied.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noun_chunks</strong></td>
<td valign="top">[<a href="#nluspan">NLUSpan</a>]</td>
<td>

The base noun phrases in the document.
    Returns a list of base noun-phrase Span objects, if the document has been syntactically parsed.
    A base noun phrase, or “NP chunk”, is a noun phrase that does not permit
other NPs to be nested within it – so no NP-level coordination, no
prepositional phrases, and no relative clauses.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentences</strong></td>
<td valign="top">[<a href="#nluspan">NLUSpan</a>]</td>
<td>

The the sentences in the document.
    Sentence spans have no label. To improve accuracy on informal texts, spaCy
calculates sentence boundaries from the syntactic dependency parse.
    If the parser is disabled, the sents iterator will be unavailable.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#nlutoken">NLUToken</a>]</td>
<td>

The tokens of the document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

### NLUSpan

A slice from a Doc object

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>entities</strong></td>
<td valign="top">[<a href="#nluspan">NLUSpan</a>]</td>
<td>

Span references

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Base form of the span, with no inflectional suffixes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#nlutoken">NLUToken</a>]</td>
<td>

Tokens within the span and tokens which descend from them.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#nlutoken">NLUToken</a>]</td>
<td>

Token references

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

### NLUToken

An individual token — i.e. a word, punctuation symbol, whitespace, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>dependency</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Syntactic dependency relation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>entity_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Named entity type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_alpha</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of alphabetic characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_ascii</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of ASCII characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_bracket</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a bracket?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_currency</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a currency symbol?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_digit</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of digits?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_left_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a left punctuation mark, e.g. "(" ?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_lower</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in lowercase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_oov</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token out-of-vocabulary (i.e. does it not have a word vector)?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token punctuation?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_quote</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a quotation mark?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_right_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a right punctuation mark, e.g. ")" ?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_sent_start</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether the token starts a sentence

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_space</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of whitespace characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_stop</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token part of a “stop list”?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_title</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in titlecase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_upper</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in uppercase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Base form of the token, with no inflectional suffixes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_email</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token resemble an email address?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_num</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token represent a number? e.g. "10.9", "10", "ten", etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_url</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token resemble a URL?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>log_probability</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Smoothed log probability estimate of token's word type (context-independent entry in the vocabulary).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The token's norm, i.e. a normalized form of the token text

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>part_of_speech</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Coarse-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#nlutoken">NLUToken</a>]</td>
<td>

A sequence containing the token and all the token’s syntactic descendants.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tag</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Fine-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

### NlpDoc

A container for accessing linguistic annotations. Access sentences and named entities.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>cats</strong></td>
<td valign="top">[<a href="#cat">Cat</a>]</td>
<td>

List of categories applied to the whole document

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The named entities in the document. Returns a list of named entity Span
objects, if the entity recognizer has been applied.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#docextension">DocExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Document ID

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>noun_chunks</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The base noun phrases in the document.
    Returns a list of base noun-phrase Span objects, if the document has been syntactically parsed.
    A base noun phrase, or “NP chunk”, is a noun phrase that does not permit
other NPs to be nested within it – so no NP-level coordination, no
prepositional phrases, and no relative clauses.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sentiment</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Sentiment score in the interval from zero to one (negative to positive)

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

The the sentences in the document.
    Sentence spans have no label. To improve accuracy on informal texts, spaCy
calculates sentence boundaries from the syntactic dependency parse.
    If the parser is disabled, the sents iterator will be unavailable.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

The tokens of the document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

### PairSimilarity

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>candidate</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Similarity sentences pair

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>input</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Similarity sentences pair

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Similarity score

</td>
</tr>
</tbody>
</table>

### Paraphrase

Paraphrasing results

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

A list of paraphrases

</td>
</tr>
</tbody>
</table>

### PhraseMatch

A phrase match

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>matched_intent</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The intent that get a match

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>similarity</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Similatiry measure

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>word_matches</strong></td>
<td valign="top">[<a href="#wordmatch">WordMatch</a>]</td>
<td>

A list of word matches

</td>
</tr>
</tbody>
</table>

### QA_Result

Answer to the given question

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td>

Question-answer result

</td>
</tr>
</tbody>
</table>

### RelationResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

Extracted relations

</td>
</tr>
</tbody>
</table>

### Result

Turn prediction result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#dialogalternative">DialogAlternative</a>]</td>
<td>

Ranked list of alternatives

</td>
</tr>
</tbody>
</table>

### ResultScores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Score of the coreference resolution for this mention

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mention text

</td>
</tr>
</tbody>
</table>

### SSMLResult

Output result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ssml</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Rendered SSML

</td>
</tr>
</tbody>
</table>

### STTResult

Output result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>alternatives</strong></td>
<td valign="top">[<a href="#textalternative">TextAlternative</a>]</td>
<td>

A list of alternatives

</td>
</tr>
</tbody>
</table>

### Scores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mention</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mention text

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Score of the coreference resolution for this mention

</td>
</tr>
</tbody>
</table>

### SentenceSimilarityScores

Sentence similarity score

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>result</strong></td>
<td valign="top">[<a href="#pairsimilarity">PairSimilarity</a>]</td>
<td>

A list of pair similarity results

</td>
</tr>
</tbody>
</table>

### SentimentAnalysisResult

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>label</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Sentiment label

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Sentiment score

</td>
</tr>
</tbody>
</table>

### ServiceInfo

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>enums</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>inputs</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interfaces</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>queries</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scalars</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### SlingDocument

SLING document

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>mentions</strong></td>
<td valign="top">[<a href="#slingmention">SlingMention</a>]</td>
<td>

List of mentions

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Document text

</td>
</tr>
</tbody>
</table>

### SlingMention

SLING mention

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>evokes</strong></td>
<td valign="top">[<a href="#string">String</a>]</td>
<td>

List of words this mention evokes

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>phrase</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Mention phrase

</td>
</tr>
</tbody>
</table>

### Span

A slice from a Doc object

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conjuncts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

A tuple of tokens coordinated to span.root.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

End position of the slice

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ents</strong></td>
<td valign="top">[<a href="#span">Span</a>]</td>
<td>

Span references

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#spanextension">SpanExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>label</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Span label

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lefts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

Tokens that are to the left of the span, whose heads are within the span.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Base form of the span, with no inflectional suffixes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rights</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

Tokens that are to the right of the span, whose heads are within the span.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>root</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td>

The token with the shortest path to the root of the sentence

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Start position of the slice

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

Tokens within the span and tokens which descend from them.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tokens</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

Token references

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

### SpanExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coref_cluster</strong></td>
<td valign="top"><a href="#corefcluster">CorefCluster</a></td>
<td>

All the clusters of corefering mentions in the doc

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>coref_scores</strong></td>
<td valign="top">[<a href="#scores">Scores</a>]</td>
<td>

Scores of the coreference resolution between mentions

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_coref</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the span a coreference?

</td>
</tr>
</tbody>
</table>

### TTSResult

Output result

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>audioB64</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Resulting audio as a base64 string

</td>
</tr>
</tbody>
</table>

### TextAlternative

Output text alternative

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>transcript</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Output text

</td>
</tr>
</tbody>
</table>

### Token

An individual token — i.e. a word, punctuation symbol, whitespace, etc.

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>ancestors</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

The rightmost token of this token’s syntactic descendants.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>children</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

A sequence of the token’s immediate syntactic children.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>cluster</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Brown cluster ID.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conjuncts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

A tuple of coordinated tokens, not including the token itself.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>dep</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Syntactic dependency relation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The ending character offset of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ent_iob</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

IOB code of named entity tag. 3 means the token begins an entity, 2 means it
is outside an entity, 1 means it is inside an entity, and 0 means no entity tag is set.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>ent_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Named entity type

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extension</strong></td>
<td valign="top"><a href="#tokenextension">TokenExtension</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>head</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td>

The syntactic parent, or "governor", of this token.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The index of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_alpha</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of alphabetic characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_ascii</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of ASCII characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_bracket</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a bracket?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_currency</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a currency symbol?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_digit</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of digits?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_left_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a left punctuation mark, e.g. "(" ?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_lower</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in lowercase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_oov</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token out-of-vocabulary (i.e. does it not have a word vector)?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token punctuation?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_quote</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a quotation mark?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_right_punct</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token a right punctuation mark, e.g. ")" ?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_sent_start</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether the token starts a sentence

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_space</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token consist of whitespace characters?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_stop</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token part of a “stop list”?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_title</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in titlecase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_upper</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in uppercase?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lang</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Language of the parent document’s vocabulary.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>left_edge</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td>

The leftmost token of this token’s syntactic descendants.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lefts</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

The leftward immediate children of the word in the syntactic dependency parse.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lemma</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Base form of the token, with no inflectional suffixes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_email</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token resemble an email address?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_num</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token represent a number? e.g. "10.9", "10", "ten", etc.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>like_url</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Does the token resemble a URL?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>lower</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Lowercase form of the token

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>norm</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

The token's norm, i.e. a normalized form of the token text

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>orth</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content (identical to Token.text).
    Exists mostly for consistency with the other attributes.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>pos</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Coarse-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Hash value of a length-N substring from the start of the token

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prob</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Smoothed log probability estimate of token's word type (context-independent entry in the vocabulary).

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>right_edge</strong></td>
<td valign="top"><a href="#token">Token</a></td>
<td>

The rightmost token of this token’s syntactic descendants.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>rights</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

The rightward immediate children of the word in the syntactic dependency parse.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>shape</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Transform of the tokens’s string to show orthographic features. Alphabetic
characters are replaced by x or X, and numeric characters are replaced by d,
and sequences of the same character are truncated after length 4. For
example,"Xxxx"or"dd"

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

The starting character offset of the token within the parent document.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>subtree</strong></td>
<td valign="top">[<a href="#token">Token</a>]</td>
<td>

A sequence containing the token and all the token’s syntactic descendants.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>suffix</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Hash value of a length-N substring from the end of the token

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>tag</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Fine-grained part-of-speech.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>whitespace</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Trailing space character if present

</td>
</tr>
</tbody>
</table>

### TokenExtension

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>coref_clusters</strong></td>
<td valign="top">[<a href="#corefcluster">CorefCluster</a>]</td>
<td>

All the clusters of corefering mentions in the doc

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>in_coref</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token in coreference?

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>is_implicit</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Is the token an implicit fused-head?

</td>
</tr>
</tbody>
</table>

### TopicScore

Topic scores

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>score</strong></td>
<td valign="top"><a href="#float">Float</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>topic</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### WordMatch

A word match

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>explanation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Match explanation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>extracted_word</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

A word extracted by the match

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>match_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Type of the match

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>similarity</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Similarity measure

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slot</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Slot filled by the match

</td>
</tr>
</tbody>
</table>

### apps

columns and relationships of "apps"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate">conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers">developers</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### apps_aggregate

aggregated selection of "apps"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#apps_aggregate_fields">apps_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### apps_aggregate_fields

aggregate fields of "apps"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#apps_avg_fields">apps_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#apps_max_fields">apps_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#apps_min_fields">apps_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#apps_stddev_fields">apps_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#apps_stddev_pop_fields">apps_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#apps_stddev_samp_fields">apps_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#apps_sum_fields">apps_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#apps_var_pop_fields">apps_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#apps_var_samp_fields">apps_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#apps_variance_fields">apps_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_mutation_response

response of any mutation on the table "apps"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### apps_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data

columns and relationships of "atomic.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_attr</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_intent</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_need</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_aggregate

aggregated selection of "atomic.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#atomic_data_aggregate_fields">atomic_data_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#atomic_data">atomic_data</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_aggregate_fields

aggregate fields of "atomic.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#atomic_data_select_column">atomic_data_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#atomic_data_max_fields">atomic_data_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#atomic_data_min_fields">atomic_data_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_mutation_response

response of any mutation on the table "atomic.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#atomic_data">atomic_data</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### audit_logged_actions

columns and relationships of "audit.logged_actions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_addr</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relid</strong></td>
<td valign="top"><a href="#oid">oid</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statement_only</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_aggregate

aggregated selection of "audit.logged_actions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#audit_logged_actions_aggregate_fields">audit_logged_actions_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#audit_logged_actions">audit_logged_actions</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_aggregate_fields

aggregate fields of "audit.logged_actions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#audit_logged_actions_avg_fields">audit_logged_actions_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#audit_logged_actions_select_column">audit_logged_actions_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#audit_logged_actions_max_fields">audit_logged_actions_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#audit_logged_actions_min_fields">audit_logged_actions_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#audit_logged_actions_stddev_fields">audit_logged_actions_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#audit_logged_actions_stddev_pop_fields">audit_logged_actions_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#audit_logged_actions_stddev_samp_fields">audit_logged_actions_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#audit_logged_actions_sum_fields">audit_logged_actions_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#audit_logged_actions_var_pop_fields">audit_logged_actions_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#audit_logged_actions_var_samp_fields">audit_logged_actions_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#audit_logged_actions_variance_fields">audit_logged_actions_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_mutation_response

response of any mutation on the table "audit.logged_actions"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#audit_logged_actions">audit_logged_actions</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### audit_logged_actions_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data

columns and relationships of "conceptnet.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_aggregate

aggregated selection of "conceptnet.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#conceptnet_data_aggregate_fields">conceptnet_data_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_aggregate_fields

aggregate fields of "conceptnet.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#conceptnet_data_avg_fields">conceptnet_data_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#conceptnet_data_max_fields">conceptnet_data_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#conceptnet_data_min_fields">conceptnet_data_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#conceptnet_data_stddev_fields">conceptnet_data_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#conceptnet_data_stddev_pop_fields">conceptnet_data_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#conceptnet_data_stddev_samp_fields">conceptnet_data_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#conceptnet_data_sum_fields">conceptnet_data_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#conceptnet_data_var_pop_fields">conceptnet_data_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#conceptnet_data_var_samp_fields">conceptnet_data_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#conceptnet_data_variance_fields">conceptnet_data_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_mutation_response

response of any mutation on the table "conceptnet.data"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### conceptnet_data_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations

columns and relationships of "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps">apps</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users">end_users</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate">end_user_conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate">utterances_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

### conversations_aggregate

aggregated selection of "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate_fields">conversations_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### conversations_aggregate_fields

aggregate fields of "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#conversations_avg_fields">conversations_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#conversations_max_fields">conversations_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#conversations_min_fields">conversations_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#conversations_stddev_fields">conversations_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#conversations_stddev_pop_fields">conversations_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#conversations_stddev_samp_fields">conversations_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#conversations_sum_fields">conversations_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#conversations_var_pop_fields">conversations_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#conversations_var_samp_fields">conversations_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#conversations_variance_fields">conversations_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_mutation_response

response of any mutation on the table "conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### conversations_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers

columns and relationships of "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>active</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps_aggregate</strong></td>
<td valign="top"><a href="#apps_aggregate">apps_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events</strong></td>
<td valign="top">[<a href="#events">events</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events_aggregate</strong></td>
<td valign="top"><a href="#events_aggregate">events_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>onboarded</strong></td>
<td valign="top"><a href="#boolean">Boolean</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### developers_aggregate

aggregated selection of "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#developers_aggregate_fields">developers_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### developers_aggregate_fields

aggregate fields of "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#developers_avg_fields">developers_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#developers_max_fields">developers_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#developers_min_fields">developers_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#developers_stddev_fields">developers_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#developers_stddev_pop_fields">developers_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#developers_stddev_samp_fields">developers_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#developers_sum_fields">developers_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#developers_var_pop_fields">developers_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#developers_var_samp_fields">developers_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#developers_variance_fields">developers_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_mutation_response

response of any mutation on the table "developers"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### developers_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations

columns and relationships of "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users">end_users</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_aggregate

aggregated selection of "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate_fields">end_user_conversations_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_aggregate_fields

aggregate fields of "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#end_user_conversations_avg_fields">end_user_conversations_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#end_user_conversations_max_fields">end_user_conversations_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#end_user_conversations_min_fields">end_user_conversations_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_fields">end_user_conversations_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_pop_fields">end_user_conversations_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_samp_fields">end_user_conversations_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#end_user_conversations_sum_fields">end_user_conversations_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#end_user_conversations_var_pop_fields">end_user_conversations_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#end_user_conversations_var_samp_fields">end_user_conversations_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#end_user_conversations_variance_fields">end_user_conversations_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_mutation_response

response of any mutation on the table "end_user_conversations"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users

columns and relationships of "end_users"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate">conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate">end_user_conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate">utterances_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### end_users_aggregate

aggregated selection of "end_users"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#end_users_aggregate_fields">end_users_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#end_users">end_users</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### end_users_aggregate_fields

aggregate fields of "end_users"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#end_users_avg_fields">end_users_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#end_users_select_column">end_users_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#end_users_max_fields">end_users_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#end_users_min_fields">end_users_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#end_users_stddev_fields">end_users_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#end_users_stddev_pop_fields">end_users_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#end_users_stddev_samp_fields">end_users_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#end_users_sum_fields">end_users_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#end_users_var_pop_fields">end_users_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#end_users_var_samp_fields">end_users_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#end_users_variance_fields">end_users_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_mutation_response

response of any mutation on the table "end_users"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#end_users">end_users</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### end_users_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### events

columns and relationships of "events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_aggregate

aggregated selection of "events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#events_aggregate_fields">events_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#events">events</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### events_aggregate_fields

aggregate fields of "events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#events_max_fields">events_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#events_min_fields">events_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_mutation_response

response of any mutation on the table "events"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#events">events</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### history

columns and relationships of "history"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_aggregate

aggregated selection of "history"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#history_aggregate_fields">history_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#history">history</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### history_aggregate_fields

aggregate fields of "history"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#history_avg_fields">history_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#history_max_fields">history_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#history_min_fields">history_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#history_stddev_fields">history_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#history_stddev_pop_fields">history_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#history_stddev_samp_fields">history_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#history_sum_fields">history_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#history_var_pop_fields">history_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#history_var_samp_fields">history_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#history_variance_fields">history_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum

columns and relationships of "kv_scope_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_aggregate

aggregated selection of "kv_scope_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#kv_scope_enum_aggregate_fields">kv_scope_enum_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#kv_scope_enum">kv_scope_enum</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_aggregate_fields

aggregate fields of "kv_scope_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#kv_scope_enum_select_column">kv_scope_enum_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#kv_scope_enum_max_fields">kv_scope_enum_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#kv_scope_enum_min_fields">kv_scope_enum_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_mutation_response

response of any mutation on the table "kv_scope_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#kv_scope_enum">kv_scope_enum</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### kv_store

columns and relationships of "kv_store"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers">developers</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
</tbody>
</table>

### kv_store_aggregate

aggregated selection of "kv_store"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate_fields">kv_store_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_aggregate_fields

aggregate fields of "kv_store"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#kv_store_avg_fields">kv_store_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#kv_store_max_fields">kv_store_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#kv_store_min_fields">kv_store_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#kv_store_stddev_fields">kv_store_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#kv_store_stddev_pop_fields">kv_store_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#kv_store_stddev_samp_fields">kv_store_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#kv_store_sum_fields">kv_store_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#kv_store_var_pop_fields">kv_store_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#kv_store_var_samp_fields">kv_store_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#kv_store_variance_fields">kv_store_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_mutation_response

response of any mutation on the table "kv_store"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### kv_store_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance

columns and relationships of "last_utterance"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_aggregate

aggregated selection of "last_utterance"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#last_utterance_aggregate_fields">last_utterance_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#last_utterance">last_utterance</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_aggregate_fields

aggregate fields of "last_utterance"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#last_utterance_avg_fields">last_utterance_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#last_utterance_max_fields">last_utterance_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#last_utterance_min_fields">last_utterance_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#last_utterance_stddev_fields">last_utterance_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#last_utterance_stddev_pop_fields">last_utterance_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#last_utterance_stddev_samp_fields">last_utterance_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#last_utterance_sum_fields">last_utterance_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#last_utterance_var_pop_fields">last_utterance_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#last_utterance_var_samp_fields">last_utterance_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#last_utterance_variance_fields">last_utterance_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects

columns and relationships of "objects"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">path</td>
<td valign="top"><a href="#string">String</a></td>
<td>

JSON select path

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### objects_aggregate

aggregated selection of "objects"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#objects_aggregate_fields">objects_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#objects">objects</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### objects_aggregate_fields

aggregate fields of "objects"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#objects_avg_fields">objects_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#objects_select_column">objects_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#objects_max_fields">objects_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#objects_min_fields">objects_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#objects_stddev_fields">objects_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#objects_stddev_pop_fields">objects_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#objects_stddev_samp_fields">objects_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#objects_sum_fields">objects_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#objects_var_pop_fields">objects_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#objects_var_samp_fields">objects_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#objects_variance_fields">objects_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_mutation_response

response of any mutation on the table "objects"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#objects">objects</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### objects_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum

columns and relationships of "speaker_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate">utterances_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_aggregate

aggregated selection of "speaker_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#speaker_type_enum_aggregate_fields">speaker_type_enum_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#speaker_type_enum">speaker_type_enum</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_aggregate_fields

aggregate fields of "speaker_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#speaker_type_enum_select_column">speaker_type_enum_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#speaker_type_enum_max_fields">speaker_type_enum_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#speaker_type_enum_min_fields">speaker_type_enum_min_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_mutation_response

response of any mutation on the table "speaker_type_enum"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#speaker_type_enum">speaker_type_enum</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### subscription_root

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top">[<a href="#apps">apps</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps_aggregate</strong></td>
<td valign="top"><a href="#apps_aggregate">apps_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#apps_select_column">apps_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#apps_order_by">apps_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>atomic_data</strong></td>
<td valign="top">[<a href="#atomic_data">atomic_data</a>!]!</td>
<td>

fetch data from the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#atomic_data_select_column">atomic_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#atomic_data_order_by">atomic_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>atomic_data_aggregate</strong></td>
<td valign="top"><a href="#atomic_data_aggregate">atomic_data_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "atomic.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#atomic_data_select_column">atomic_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#atomic_data_order_by">atomic_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions</strong></td>
<td valign="top">[<a href="#audit_logged_actions">audit_logged_actions</a>!]!</td>
<td>

fetch data from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#audit_logged_actions_select_column">audit_logged_actions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#audit_logged_actions_order_by">audit_logged_actions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions_aggregate</strong></td>
<td valign="top"><a href="#audit_logged_actions_aggregate">audit_logged_actions_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "audit.logged_actions"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#audit_logged_actions_select_column">audit_logged_actions_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#audit_logged_actions_order_by">audit_logged_actions_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>audit_logged_actions_by_pk</strong></td>
<td valign="top"><a href="#audit_logged_actions">audit_logged_actions</a></td>
<td>

fetch data from the table: "audit.logged_actions" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">action_tstamp_stm</td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">event_id</td>
<td valign="top"><a href="#bigint">bigint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_data</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td>

fetch data from the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_data_aggregate</strong></td>
<td valign="top"><a href="#conceptnet_data_aggregate">conceptnet_data_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_search_relations</strong></td>
<td valign="top">[<a href="#conceptnet_data">conceptnet_data</a>!]!</td>
<td>

execute function "conceptnet.search_relations" which returns "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">args</td>
<td valign="top"><a href="#conceptnet_search_relations_args">conceptnet_search_relations_args</a>!</td>
<td>

input parameters for function "conceptnet.search_relations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conceptnet_search_relations_aggregate</strong></td>
<td valign="top"><a href="#conceptnet_data_aggregate">conceptnet_data_aggregate</a>!</td>
<td>

execute function "conceptnet.search_relations" and query aggregates on result of table type "conceptnet.data"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">args</td>
<td valign="top"><a href="#conceptnet_search_relations_args">conceptnet_search_relations_args</a>!</td>
<td>

input parameters for function "conceptnet.search_relations"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conceptnet_data_select_column">conceptnet_data_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conceptnet_data_order_by">conceptnet_data_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top">[<a href="#conversations">conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate">conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#conversations_select_column">conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#conversations_order_by">conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

fetch data from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developers_aggregate</strong></td>
<td valign="top"><a href="#developers_aggregate">developers_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top">[<a href="#end_user_conversations">end_user_conversations</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate">end_user_conversations_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_user_conversations_select_column">end_user_conversations_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_user_conversations_order_by">end_user_conversations_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_by_pk</strong></td>
<td valign="top"><a href="#end_user_conversations">end_user_conversations</a></td>
<td>

fetch data from the table: "end_user_conversations" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">conversation_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">end_user_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_users</strong></td>
<td valign="top">[<a href="#end_users">end_users</a>!]!</td>
<td>

fetch data from the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_users_select_column">end_users_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_users_order_by">end_users_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_users_aggregate</strong></td>
<td valign="top"><a href="#end_users_aggregate">end_users_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "end_users"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#end_users_select_column">end_users_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#end_users_order_by">end_users_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events</strong></td>
<td valign="top">[<a href="#events">events</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events_aggregate</strong></td>
<td valign="top"><a href="#events_aggregate">events_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#events_select_column">events_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#events_order_by">events_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history</strong></td>
<td valign="top">[<a href="#history">history</a>!]!</td>
<td>

fetch data from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>history_aggregate</strong></td>
<td valign="top"><a href="#history_aggregate">history_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "history"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#history_select_column">history_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#history_order_by">history_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum</strong></td>
<td valign="top">[<a href="#kv_scope_enum">kv_scope_enum</a>!]!</td>
<td>

fetch data from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_scope_enum_select_column">kv_scope_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_scope_enum_order_by">kv_scope_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum_aggregate</strong></td>
<td valign="top"><a href="#kv_scope_enum_aggregate">kv_scope_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "kv_scope_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_scope_enum_select_column">kv_scope_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_scope_enum_order_by">kv_scope_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_scope_enum_by_pk</strong></td>
<td valign="top"><a href="#kv_scope_enum">kv_scope_enum</a></td>
<td>

fetch data from the table: "kv_scope_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top">[<a href="#kv_store">kv_store</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate">kv_store_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#kv_store_select_column">kv_store_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#kv_store_order_by">kv_store_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_by_pk</strong></td>
<td valign="top"><a href="#kv_store">kv_store</a></td>
<td>

fetch data from the table: "kv_store" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">key</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">scope_object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance</strong></td>
<td valign="top">[<a href="#last_utterance">last_utterance</a>!]!</td>
<td>

fetch data from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>last_utterance_aggregate</strong></td>
<td valign="top"><a href="#last_utterance_aggregate">last_utterance_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "last_utterance"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#last_utterance_select_column">last_utterance_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#last_utterance_order_by">last_utterance_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>me</strong></td>
<td valign="top">[<a href="#developers">developers</a>!]!</td>
<td>

execute function "me" which returns "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>me_aggregate</strong></td>
<td valign="top"><a href="#developers_aggregate">developers_aggregate</a>!</td>
<td>

execute function "me" and query aggregates on result of table type "developers"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#developers_select_column">developers_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#developers_order_by">developers_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects</strong></td>
<td valign="top">[<a href="#objects">objects</a>!]!</td>
<td>

fetch data from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#objects_select_column">objects_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#objects_order_by">objects_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects_aggregate</strong></td>
<td valign="top"><a href="#objects_aggregate">objects_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "objects"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#objects_select_column">objects_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#objects_order_by">objects_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>objects_by_pk</strong></td>
<td valign="top"><a href="#objects">objects</a></td>
<td>

fetch data from the table: "objects" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">object_id</td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top">[<a href="#speaker_type_enum">speaker_type_enum</a>!]!</td>
<td>

fetch data from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#speaker_type_enum_select_column">speaker_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#speaker_type_enum_order_by">speaker_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum_aggregate</strong></td>
<td valign="top"><a href="#speaker_type_enum_aggregate">speaker_type_enum_aggregate</a>!</td>
<td>

fetch aggregated fields from the table: "speaker_type_enum"

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#speaker_type_enum_select_column">speaker_type_enum_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#speaker_type_enum_order_by">speaker_type_enum_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum_by_pk</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a></td>
<td>

fetch data from the table: "speaker_type_enum" using primary key columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">value</td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

An array relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate">utterances_aggregate</a>!</td>
<td>

An aggregate relationship

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct_on</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td>

distinct select on columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">limit</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

limit the number of rows returned

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">offset</td>
<td valign="top"><a href="#int">Int</a></td>
<td>

skip the first n rows. Use only with order_by

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">order_by</td>
<td valign="top">[<a href="#utterances_order_by">utterances_order_by</a>!]</td>
<td>

sort the rows by one or more columns

</td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">where</td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td>

filter the rows returned

</td>
</tr>
</tbody>
</table>

### utterances

columns and relationships of "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations">conversations</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users">end_users</a></td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum">speaker_type_enum</a>!</td>
<td>

An object relationship

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### utterances_aggregate

aggregated selection of "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate_fields">utterances_aggregate_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>nodes</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### utterances_aggregate_fields

aggregate fields of "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#utterances_avg_fields">utterances_avg_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">columns</td>
<td valign="top">[<a href="#utterances_select_column">utterances_select_column</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" align="right" valign="top">distinct</td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#utterances_max_fields">utterances_max_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#utterances_min_fields">utterances_min_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#utterances_stddev_fields">utterances_stddev_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#utterances_stddev_pop_fields">utterances_stddev_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#utterances_stddev_samp_fields">utterances_stddev_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#utterances_sum_fields">utterances_sum_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#utterances_var_pop_fields">utterances_var_pop_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#utterances_var_samp_fields">utterances_var_samp_fields</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#utterances_variance_fields">utterances_variance_fields</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_avg_fields

aggregate avg on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_max_fields

aggregate max on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_min_fields

aggregate min on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_mutation_response

response of any mutation on the table "utterances"

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>affected_rows</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td>

number of rows affected by the mutation

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>returning</strong></td>
<td valign="top">[<a href="#utterances">utterances</a>!]!</td>
<td>

data from the rows affected by the mutation

</td>
</tr>
</tbody>
</table>

### utterances_stddev_fields

aggregate stddev on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_stddev_pop_fields

aggregate stddev_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_stddev_samp_fields

aggregate stddev_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_sum_fields

aggregate sum on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_var_pop_fields

aggregate var_pop on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_var_samp_fields

aggregate var_samp on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_variance_fields

aggregate variance on columns

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td></td>
</tr>
</tbody>
</table>

## Inputs

### Boolean_comparison_exp

Boolean expression to compare columns of type "Boolean". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#boolean">Boolean</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#boolean">Boolean</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### ContextObject

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>content</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Dialog turn content

</td>
</tr>
</tbody>
</table>

### InputPipe

Pipe input type

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>context</strong></td>
<td valign="top"><a href="#json">JSON</a></td>
<td>

Variable bindings

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>op</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Service query name

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transform</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Transform logic

</td>
</tr>
</tbody>
</table>

### Int_comparison_exp

Boolean expression to compare columns of type "Int". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#int">Int</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### STTConfig

Speech to text config

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>encoding</strong></td>
<td valign="top"><a href="#encoding">Encoding</a></td>
<td>

Audio encoding

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Language code

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>maxAlternatives</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Maximum number of the output alternatives

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>profanityFilter</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

Profanity filter flag

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sampleRate</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td>

Audio Sample rate

</td>
</tr>
</tbody>
</table>

### String_comparison_exp

Boolean expression to compare columns of type "String". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_ilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given case-insensitive pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_iregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given POSIX regular expression, case insensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_like</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nilike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given case-insensitive pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_niregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given POSIX regular expression, case insensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nlike</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given pattern

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nregex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given POSIX regular expression, case sensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nsimilar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column NOT match the given SQL regular expression

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_regex</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given POSIX regular expression, case sensitive

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_similar</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the column match the given SQL regular expression

</td>
</tr>
</tbody>
</table>

### TTSConfig

Input config

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>encoding</strong></td>
<td valign="top"><a href="#audioencoding">AudioEncoding</a></td>
<td>

Audio encoding

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>languageCode</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Language code

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sampleRate</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

Audio sample rate

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>voiceGender</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Voice gender

</td>
</tr>
</tbody>
</table>

### Turn

An object representing a single turn by an agent

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>agent</strong></td>
<td valign="top"><a href="#agent">Agent</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>said</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### _text_comparison_exp

Boolean expression to compare columns of type "_text". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#_text">_text</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#_text">_text</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### app_status_comparison_exp

Boolean expression to compare columns of type "app_status". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#app_status">app_status</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#app_status">app_status</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### apps_aggregate_order_by

order by aggregate values of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#apps_avg_order_by">apps_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#apps_max_order_by">apps_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#apps_min_order_by">apps_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#apps_stddev_order_by">apps_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#apps_stddev_pop_order_by">apps_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#apps_stddev_samp_order_by">apps_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#apps_sum_order_by">apps_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#apps_var_pop_order_by">apps_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#apps_var_samp_order_by">apps_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#apps_variance_order_by">apps_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_arr_rel_insert_input

input type for inserting array relation for remote table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#apps_insert_input">apps_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### apps_avg_order_by

order by avg() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_bool_exp

Boolean expression to filter rows from the table "apps". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#apps_bool_exp">apps_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#apps_bool_exp">apps_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status_comparison_exp">app_status_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### apps_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_inc_input

input type for incrementing numeric columns in table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_insert_input

input type for inserting data into table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_arr_rel_insert_input">conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_obj_rel_insert_input">developers_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_arr_rel_insert_input">kv_store_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_max_order_by

order by max() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_min_order_by

order by min() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_obj_rel_insert_input

input type for inserting object relation for remote table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#apps_insert_input">apps_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#apps_on_conflict">apps_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### apps_on_conflict

on conflict condition type for table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#apps_constraint">apps_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#apps_update_column">apps_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_order_by

Ordering options when selecting data from "apps".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate_order_by">conversations_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_order_by">developers_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate_order_by">kv_store_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_set_input

input type for updating data in table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>slug</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>status</strong></td>
<td valign="top"><a href="#app_status">app_status</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_stddev_order_by

order by stddev() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_stddev_pop_order_by

order by stddev_pop() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_stddev_samp_order_by

order by stddev_samp() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_sum_order_by

order by sum() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_var_pop_order_by

order by var_pop() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_var_samp_order_by

order by var_samp() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### apps_variance_order_by

order by variance() on columns of table "apps"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_bool_exp

Boolean expression to filter rows from the table "atomic.data". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#atomic_data_bool_exp">atomic_data_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#atomic_data_bool_exp">atomic_data_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#atomic_data_bool_exp">atomic_data_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_effect</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_react</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_want</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_attr</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_effect</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_intent</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_need</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_react</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_want</strong></td>
<td valign="top"><a href="#_text_comparison_exp">_text_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_insert_input

input type for inserting data into table "atomic.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_attr</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_intent</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_need</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_order_by

Ordering options when selecting data from "atomic.data".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_effect</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_react</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_want</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_attr</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_effect</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_intent</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_need</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_react</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_want</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### atomic_data_set_input

input type for updating data in table "atomic.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>event</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>o_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>prefix</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_attr</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_effect</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_intent</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_need</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_react</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>x_want</strong></td>
<td valign="top"><a href="#_text">_text</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_bool_exp

Boolean expression to filter rows from the table "audit.logged_actions". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_addr</strong></td>
<td valign="top"><a href="#inet_comparison_exp">inet_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint_comparison_exp">bigint_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relid</strong></td>
<td valign="top"><a href="#oid_comparison_exp">oid_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statement_only</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint_comparison_exp">bigint_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_inc_input

input type for incrementing numeric columns in table "audit.logged_actions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_insert_input

input type for inserting data into table "audit.logged_actions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_addr</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relid</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statement_only</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_on_conflict

on conflict condition type for table "audit.logged_actions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#audit_logged_actions_constraint">audit_logged_actions_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#audit_logged_actions_update_column">audit_logged_actions_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#audit_logged_actions_bool_exp">audit_logged_actions_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_order_by

Ordering options when selecting data from "audit.logged_actions".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_addr</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relid</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statement_only</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_pk_columns_input

primary key columns input for table: audit_logged_actions

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### audit_logged_actions_set_input

input type for updating data in table "audit.logged_actions"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_clk</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_stm</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action_tstamp_tx</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>application_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_addr</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_port</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>client_query</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>event_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>hasura_user</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relid</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>row_data</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>schema_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>session_user_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>statement_only</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>transaction_id</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
</tbody>
</table>

### bigint_comparison_exp

Boolean expression to compare columns of type "bigint". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#bigint">bigint</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#bigint">bigint</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#bigint">bigint</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_bool_exp

Boolean expression to filter rows from the table "conceptnet.data". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric_comparison_exp">numeric_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_inc_input

input type for incrementing numeric columns in table "conceptnet.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_insert_input

input type for inserting data into table "conceptnet.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_on_conflict

on conflict condition type for table "conceptnet.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#conceptnet_data_constraint">conceptnet_data_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#conceptnet_data_update_column">conceptnet_data_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#conceptnet_data_bool_exp">conceptnet_data_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_order_by

Ordering options when selecting data from "conceptnet.data".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_data_set_input

input type for updating data in table "conceptnet.data"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>end</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>relation</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>start</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uri</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>weight</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
</tbody>
</table>

### conceptnet_search_relations_args

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>limit_to</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>search</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_aggregate_order_by

order by aggregate values of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#conversations_avg_order_by">conversations_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#conversations_max_order_by">conversations_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#conversations_min_order_by">conversations_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#conversations_stddev_order_by">conversations_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#conversations_stddev_pop_order_by">conversations_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#conversations_stddev_samp_order_by">conversations_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#conversations_sum_order_by">conversations_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#conversations_var_pop_order_by">conversations_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#conversations_var_samp_order_by">conversations_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#conversations_variance_order_by">conversations_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_arr_rel_insert_input

input type for inserting array relation for remote table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#conversations_insert_input">conversations_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### conversations_avg_order_by

order by avg() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_bool_exp

Boolean expression to filter rows from the table "conversations". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#conversations_bool_exp">conversations_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#conversations_bool_exp">conversations_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### conversations_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_inc_input

input type for incrementing numeric columns in table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_insert_input

input type for inserting data into table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_obj_rel_insert_input">apps_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_obj_rel_insert_input">end_users_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_arr_rel_insert_input">end_user_conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_arr_rel_insert_input">kv_store_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_arr_rel_insert_input">utterances_arr_rel_insert_input</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_max_order_by

order by max() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_min_order_by

order by min() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_obj_rel_insert_input

input type for inserting object relation for remote table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#conversations_insert_input">conversations_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#conversations_on_conflict">conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### conversations_on_conflict

on conflict condition type for table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#conversations_constraint">conversations_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#conversations_update_column">conversations_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_order_by

Ordering options when selecting data from "conversations".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app</strong></td>
<td valign="top"><a href="#apps_order_by">apps_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_order_by">end_users_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate_order_by">end_user_conversations_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate_order_by">kv_store_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate_order_by">utterances_aggregate_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_set_input

input type for updating data in table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>destroyed_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_stddev_order_by

order by stddev() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_stddev_pop_order_by

order by stddev_pop() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_stddev_samp_order_by

order by stddev_samp() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_sum_order_by

order by sum() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_var_pop_order_by

order by var_pop() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_var_samp_order_by

order by var_samp() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### conversations_variance_order_by

order by variance() on columns of table "conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>app_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_bool_exp

Boolean expression to filter rows from the table "developers". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#developers_bool_exp">developers_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#developers_bool_exp">developers_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>active</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top"><a href="#apps_bool_exp">apps_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events</strong></td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>onboarded</strong></td>
<td valign="top"><a href="#boolean_comparison_exp">Boolean_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### developers_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_inc_input

input type for incrementing numeric columns in table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_insert_input

input type for inserting data into table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>active</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps</strong></td>
<td valign="top"><a href="#apps_arr_rel_insert_input">apps_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events</strong></td>
<td valign="top"><a href="#events_arr_rel_insert_input">events_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores</strong></td>
<td valign="top"><a href="#kv_store_arr_rel_insert_input">kv_store_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>onboarded</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_obj_rel_insert_input

input type for inserting object relation for remote table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#developers_insert_input">developers_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#developers_on_conflict">developers_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### developers_on_conflict

on conflict condition type for table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#developers_constraint">developers_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#developers_update_column">developers_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_order_by

Ordering options when selecting data from "developers".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>active</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>apps_aggregate</strong></td>
<td valign="top"><a href="#apps_aggregate_order_by">apps_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>events_aggregate</strong></td>
<td valign="top"><a href="#events_aggregate_order_by">events_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_stores_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate_order_by">kv_store_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>onboarded</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### developers_set_input

input type for updating data in table "developers"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>active</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>api_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>email</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>github_handle</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>onboarded</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_aggregate_order_by

order by aggregate values of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#end_user_conversations_avg_order_by">end_user_conversations_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#end_user_conversations_max_order_by">end_user_conversations_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#end_user_conversations_min_order_by">end_user_conversations_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_order_by">end_user_conversations_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_pop_order_by">end_user_conversations_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#end_user_conversations_stddev_samp_order_by">end_user_conversations_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#end_user_conversations_sum_order_by">end_user_conversations_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#end_user_conversations_var_pop_order_by">end_user_conversations_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#end_user_conversations_var_samp_order_by">end_user_conversations_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#end_user_conversations_variance_order_by">end_user_conversations_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_arr_rel_insert_input

input type for inserting array relation for remote table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#end_user_conversations_insert_input">end_user_conversations_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#end_user_conversations_on_conflict">end_user_conversations_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### end_user_conversations_avg_order_by

order by avg() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_bool_exp

Boolean expression to filter rows from the table "end_user_conversations". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_inc_input

input type for incrementing numeric columns in table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_insert_input

input type for inserting data into table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_obj_rel_insert_input">conversations_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_obj_rel_insert_input">end_users_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_max_order_by

order by max() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_min_order_by

order by min() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_on_conflict

on conflict condition type for table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#end_user_conversations_constraint">end_user_conversations_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#end_user_conversations_update_column">end_user_conversations_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_order_by

Ordering options when selecting data from "end_user_conversations".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_order_by">end_users_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_pk_columns_input

primary key columns input for table: end_user_conversations

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_set_input

input type for updating data in table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_order_by

order by stddev() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_pop_order_by

order by stddev_pop() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_stddev_samp_order_by

order by stddev_samp() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_sum_order_by

order by sum() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_var_pop_order_by

order by var_pop() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_var_samp_order_by

order by var_samp() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_user_conversations_variance_order_by

order by variance() on columns of table "end_user_conversations"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_bool_exp

Boolean expression to filter rows from the table "end_users". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#end_users_bool_exp">end_users_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#end_users_bool_exp">end_users_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_bool_exp">end_user_conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### end_users_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_inc_input

input type for incrementing numeric columns in table "end_users"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_insert_input

input type for inserting data into table "end_users"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations</strong></td>
<td valign="top"><a href="#conversations_arr_rel_insert_input">conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations</strong></td>
<td valign="top"><a href="#end_user_conversations_arr_rel_insert_input">end_user_conversations_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store</strong></td>
<td valign="top"><a href="#kv_store_arr_rel_insert_input">kv_store_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_arr_rel_insert_input">utterances_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_obj_rel_insert_input

input type for inserting object relation for remote table "end_users"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#end_users_insert_input">end_users_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#end_users_on_conflict">end_users_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### end_users_on_conflict

on conflict condition type for table "end_users"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#end_users_constraint">end_users_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#end_users_update_column">end_users_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_order_by

Ordering options when selecting data from "end_users".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversations_aggregate</strong></td>
<td valign="top"><a href="#conversations_aggregate_order_by">conversations_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_conversations_aggregate</strong></td>
<td valign="top"><a href="#end_user_conversations_aggregate_order_by">end_user_conversations_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>kv_store_aggregate</strong></td>
<td valign="top"><a href="#kv_store_aggregate_order_by">kv_store_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate_order_by">utterances_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### end_users_set_input

input type for updating data in table "end_users"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_name</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>uuid</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_aggregate_order_by

order by aggregate values of table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#events_max_order_by">events_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#events_min_order_by">events_min_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_arr_rel_insert_input

input type for inserting array relation for remote table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#events_insert_input">events_insert_input</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### events_bool_exp

Boolean expression to filter rows from the table "events". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#events_bool_exp">events_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#events_bool_exp">events_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#events_bool_exp">events_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### events_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_insert_input

input type for inserting data into table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_max_order_by

order by max() on columns of table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_min_order_by

order by min() on columns of table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_order_by

Ordering options when selecting data from "events".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### events_set_input

input type for updating data in table "events"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>action</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>changed_fields</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer_id</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>table</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_bool_exp

Boolean expression to filter rows from the table "history". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#history_bool_exp">history_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#history_bool_exp">history_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#history_bool_exp">history_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#tstzrange_comparison_exp">tstzrange_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### history_order_by

Ordering options when selecting data from "history".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>window</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### inet_comparison_exp

Boolean expression to compare columns of type "inet". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#inet">inet</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#inet">inet</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#inet">inet</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### jsonb_comparison_exp

Boolean expression to compare columns of type "jsonb". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_contained_in</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td>

is the column contained in the given json value

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_contains</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td>

does the column contain the given json value at the top level

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

does the string exist as a top-level key in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_keys_all</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td>

do all of these strings exist as top-level keys in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_has_keys_any</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td>

do any of these strings exist as top-level keys in the column

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#jsonb">jsonb</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#jsonb">jsonb</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_bool_exp

Boolean expression to filter rows from the table "kv_scope_enum". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_insert_input

input type for inserting data into table "kv_scope_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_on_conflict

on conflict condition type for table "kv_scope_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#kv_scope_enum_constraint">kv_scope_enum_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#kv_scope_enum_update_column">kv_scope_enum_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#kv_scope_enum_bool_exp">kv_scope_enum_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_order_by

Ordering options when selecting data from "kv_scope_enum".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_pk_columns_input

primary key columns input for table: kv_scope_enum

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### kv_scope_enum_set_input

input type for updating data in table "kv_scope_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_aggregate_order_by

order by aggregate values of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#kv_store_avg_order_by">kv_store_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#kv_store_max_order_by">kv_store_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#kv_store_min_order_by">kv_store_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#kv_store_stddev_order_by">kv_store_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#kv_store_stddev_pop_order_by">kv_store_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#kv_store_stddev_samp_order_by">kv_store_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#kv_store_sum_order_by">kv_store_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#kv_store_var_pop_order_by">kv_store_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#kv_store_var_samp_order_by">kv_store_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#kv_store_variance_order_by">kv_store_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_arr_rel_insert_input

input type for inserting array relation for remote table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#kv_store_insert_input">kv_store_insert_input</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#kv_store_on_conflict">kv_store_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### kv_store_avg_order_by

order by avg() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_bool_exp

Boolean expression to filter rows from the table "kv_store". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#kv_store_bool_exp">kv_store_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#kv_store_bool_exp">kv_store_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_bool_exp">developers_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_inc_input

input type for incrementing numeric columns in table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_insert_input

input type for inserting data into table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_obj_rel_insert_input">developers_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_max_order_by

order by max() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_min_order_by

order by min() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_on_conflict

on conflict condition type for table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#kv_store_constraint">kv_store_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#kv_store_update_column">kv_store_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#kv_store_bool_exp">kv_store_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_order_by

Ordering options when selecting data from "kv_store".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>developer</strong></td>
<td valign="top"><a href="#developers_order_by">developers_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_pk_columns_input

primary key columns input for table: kv_store

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_set_input

input type for updating data in table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>key</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_stddev_order_by

order by stddev() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_stddev_pop_order_by

order by stddev_pop() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_stddev_samp_order_by

order by stddev_samp() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_sum_order_by

order by sum() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_var_pop_order_by

order by var_pop() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_var_samp_order_by

order by var_samp() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### kv_store_variance_order_by

order by variance() on columns of table "kv_store"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_by</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>scope_object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_bool_exp

Boolean expression to filter rows from the table "last_utterance". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#last_utterance_bool_exp">last_utterance_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#last_utterance_bool_exp">last_utterance_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#last_utterance_bool_exp">last_utterance_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### last_utterance_order_by

Ordering options when selecting data from "last_utterance".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>interval</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>updated_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### numeric_comparison_exp

Boolean expression to compare columns of type "numeric". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#numeric">numeric</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#numeric">numeric</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#numeric">numeric</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### objects_append_input

append existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_bool_exp

Boolean expression to filter rows from the table "objects". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#objects_bool_exp">objects_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#objects_bool_exp">objects_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb_comparison_exp">jsonb_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_delete_at_path_input

delete the field or element with specified path (for JSON arrays, negative integers count from the end)

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top">[<a href="#string">String</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### objects_delete_elem_input

delete the array element with specified index (negative integers count from the
end). throws an error if top level container is not an array

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_delete_key_input

delete key/value pair or string element. key/value pairs are matched based on their key value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_inc_input

input type for incrementing numeric columns in table "objects"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_insert_input

input type for inserting data into table "objects"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_on_conflict

on conflict condition type for table "objects"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#objects_constraint">objects_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#objects_update_column">objects_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#objects_bool_exp">objects_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_order_by

Ordering options when selecting data from "objects".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_pk_columns_input

primary key columns input for table: objects

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### objects_prepend_input

prepend existing jsonb value of filtered columns with new jsonb value

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
</tbody>
</table>

### objects_set_input

input type for updating data in table "objects"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>created_at</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>metadata</strong></td>
<td valign="top"><a href="#jsonb">jsonb</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>object_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### oid_comparison_exp

Boolean expression to compare columns of type "oid". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#oid">oid</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#oid">oid</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#oid">oid</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_bool_exp

Boolean expression to filter rows from the table "speaker_type_enum". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_enum_comparison_exp

Boolean expression to compare columns of type "speaker_type_enum_enum". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#speaker_type_enum_enum">speaker_type_enum_enum</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_insert_input

input type for inserting data into table "speaker_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>utterances</strong></td>
<td valign="top"><a href="#utterances_arr_rel_insert_input">utterances_arr_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_obj_rel_insert_input

input type for inserting object relation for remote table "speaker_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top"><a href="#speaker_type_enum_insert_input">speaker_type_enum_insert_input</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>on_conflict</strong></td>
<td valign="top"><a href="#speaker_type_enum_on_conflict">speaker_type_enum_on_conflict</a></td>
<td>

on conflict condition

</td>
</tr>
</tbody>
</table>

### speaker_type_enum_on_conflict

on conflict condition type for table "speaker_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>constraint</strong></td>
<td valign="top"><a href="#speaker_type_enum_constraint">speaker_type_enum_constraint</a>!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>update_columns</strong></td>
<td valign="top">[<a href="#speaker_type_enum_update_column">speaker_type_enum_update_column</a>!]!</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>where</strong></td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_order_by

Ordering options when selecting data from "speaker_type_enum".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>utterances_aggregate</strong></td>
<td valign="top"><a href="#utterances_aggregate_order_by">utterances_aggregate_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_pk_columns_input

primary key columns input for table: speaker_type_enum

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a>!</td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_set_input

input type for updating data in table "speaker_type_enum"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>value</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### timestamptz_comparison_exp

Boolean expression to compare columns of type "timestamptz". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#timestamptz">timestamptz</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### tstzrange_comparison_exp

Boolean expression to compare columns of type "tstzrange". All fields are combined with logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_eq</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gt</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_gte</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_in</strong></td>
<td valign="top">[<a href="#tstzrange">tstzrange</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_is_null</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lt</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_lte</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_neq</strong></td>
<td valign="top"><a href="#tstzrange">tstzrange</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_nin</strong></td>
<td valign="top">[<a href="#tstzrange">tstzrange</a>!]</td>
<td></td>
</tr>
</tbody>
</table>

### utterances_aggregate_order_by

order by aggregate values of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>avg</strong></td>
<td valign="top"><a href="#utterances_avg_order_by">utterances_avg_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>count</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>max</strong></td>
<td valign="top"><a href="#utterances_max_order_by">utterances_max_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>min</strong></td>
<td valign="top"><a href="#utterances_min_order_by">utterances_min_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev</strong></td>
<td valign="top"><a href="#utterances_stddev_order_by">utterances_stddev_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_pop</strong></td>
<td valign="top"><a href="#utterances_stddev_pop_order_by">utterances_stddev_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>stddev_samp</strong></td>
<td valign="top"><a href="#utterances_stddev_samp_order_by">utterances_stddev_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>sum</strong></td>
<td valign="top"><a href="#utterances_sum_order_by">utterances_sum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_pop</strong></td>
<td valign="top"><a href="#utterances_var_pop_order_by">utterances_var_pop_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>var_samp</strong></td>
<td valign="top"><a href="#utterances_var_samp_order_by">utterances_var_samp_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>variance</strong></td>
<td valign="top"><a href="#utterances_variance_order_by">utterances_variance_order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_arr_rel_insert_input

input type for inserting array relation for remote table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>data</strong></td>
<td valign="top">[<a href="#utterances_insert_input">utterances_insert_input</a>!]!</td>
<td></td>
</tr>
</tbody>
</table>

### utterances_avg_order_by

order by avg() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_bool_exp

Boolean expression to filter rows from the table "utterances". All fields are combined with a logical 'AND'.

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>_and</strong></td>
<td valign="top">[<a href="#utterances_bool_exp">utterances_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_not</strong></td>
<td valign="top"><a href="#utterances_bool_exp">utterances_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>_or</strong></td>
<td valign="top">[<a href="#utterances_bool_exp">utterances_bool_exp</a>!]</td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_bool_exp">conversations_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_bool_exp">end_users_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int_comparison_exp">Int_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum_comparison_exp">speaker_type_enum_enum_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_bool_exp">speaker_type_enum_bool_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz_comparison_exp">timestamptz_comparison_exp</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string_comparison_exp">String_comparison_exp</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_inc_input

input type for incrementing numeric columns in table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_insert_input

input type for inserting data into table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_obj_rel_insert_input">conversations_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_obj_rel_insert_input">end_users_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_obj_rel_insert_input">speaker_type_enum_obj_rel_insert_input</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_max_order_by

order by max() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_min_order_by

order by min() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_order_by

Ordering options when selecting data from "utterances".

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation</strong></td>
<td valign="top"><a href="#conversations_order_by">conversations_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user</strong></td>
<td valign="top"><a href="#end_users_order_by">end_users_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type_enum</strong></td>
<td valign="top"><a href="#speaker_type_enum_order_by">speaker_type_enum_order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_set_input

input type for updating data in table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#int">Int</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>normalized_utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>speaker_type</strong></td>
<td valign="top"><a href="#speaker_type_enum_enum">speaker_type_enum_enum</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>timestamp</strong></td>
<td valign="top"><a href="#timestamptz">timestamptz</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>utterance</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_stddev_order_by

order by stddev() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_stddev_pop_order_by

order by stddev_pop() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_stddev_samp_order_by

order by stddev_samp() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_sum_order_by

order by sum() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_var_pop_order_by

order by var_pop() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_var_samp_order_by

order by var_samp() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

### utterances_variance_order_by

order by variance() on columns of table "utterances"

<table>
<thead>
<tr>
<th colspan="2" align="left">Field</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>conversation_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>end_user_id</strong></td>
<td valign="top"><a href="#order_by">order_by</a></td>
<td></td>
</tr>
</tbody>
</table>

## Enums

### ACEOutputType

Output format

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>drs</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drshtml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drspp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>drsxml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>fol</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlfss</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlfsspp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlrdf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>owlxml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase1</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase2</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>pnf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ruleml</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntax</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxd</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxdpp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>syntaxpp</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>tokens</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>tptp</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Agent

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>BOT</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>USER</strong></td>
<td></td>
</tr>
</tbody>
</table>

### AudioEncoding

Audio encoding

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AUDIO_ENCODING_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LINEAR16</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MP3</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OGG_OPUS</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Category

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>oEffect</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>oReact</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>oWant</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xAttr</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xEffect</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xIntent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xNeed</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xReact</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>xWant</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Encoding

Audio encoding

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AMR</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>AMR_WB</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ENCODING_UNSPECIFIED</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>FLAC</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LINEAR16</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MP3</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MULAW</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>OGG_OPUS</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SPEEX_WITH_HEADER_BYTE</strong></td>
<td></td>
</tr>
</tbody>
</table>

### Relation

Relation type

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>AtLocation</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CapableOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Causes</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CausesDesire</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>CreatedBy</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DefinedAs</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>DesireOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>Desires</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasA</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasFirstSubevent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasLastSubevent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasPainCharacter</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasPainIntensity</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasPrerequisite</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasProperty</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>HasSubevent</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>InheritsFrom</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>InstanceOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>IsA</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LocatedNear</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>LocationOfAction</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MadeOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>MotivatedByGoal</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotCapableOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotDesires</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotHasA</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotHasProperty</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotIsA</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>NotMadeOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>PartOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>ReceivesAction</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>RelatedTo</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>SymbolOf</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>UsedFor</strong></td>
<td></td>
</tr>
</tbody>
</table>

### ServiceName

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>ace_parser</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>chitchat_service</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>commonsense</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>compose_services</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>context_frame_parser</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>docs</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>faq_service</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>intent_matcher</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>nlu_service</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>paraphrase_sentences</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>sentence_similarity</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>speech_to_text</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>text_to_speech</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>topic_classification</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>turn_prediction</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>voice_css_render</strong></td>
<td></td>
</tr>
</tbody>
</table>

### apps_constraint

unique or primary key constraints on table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>apps_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>apps_slug_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### apps_select_column

select columns of table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>developer_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>slug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### apps_update_column

update columns of table "apps"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>developer_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>slug</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>status</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### atomic_data_select_column

select columns of table "atomic.data"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>event</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>o_effect</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>o_react</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>o_want</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>prefix</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_attr</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_effect</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_intent</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_need</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_react</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>x_want</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### audit_logged_actions_constraint

unique or primary key constraints on table "audit.logged_actions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>logged_actions_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### audit_logged_actions_select_column

select columns of table "audit.logged_actions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>action</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_clk</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_stm</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_tx</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>application_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>changed_fields</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_addr</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_port</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_query</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>hasura_user</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>relid</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>row_data</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>schema_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>session_user_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>statement_only</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>table_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>transaction_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### audit_logged_actions_update_column

update columns of table "audit.logged_actions"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>action</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_clk</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_stm</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>action_tstamp_tx</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>application_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>changed_fields</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_addr</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_port</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>client_query</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>event_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>hasura_user</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>relid</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>row_data</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>schema_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>session_user_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>statement_only</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>table_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>transaction_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### conceptnet_data_constraint

unique or primary key constraints on table "conceptnet.data"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>data_start_relation_end_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>data_uri_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### conceptnet_data_select_column

select columns of table "conceptnet.data"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>end</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>relation</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>start</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uri</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>weight</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### conceptnet_data_update_column

update columns of table "conceptnet.data"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>end</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>relation</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>start</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uri</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>weight</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### conversations_constraint

unique or primary key constraints on table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversations_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### conversations_select_column

select columns of table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>app_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>destroyed_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### conversations_update_column

update columns of table "conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>app_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>destroyed_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### developers_constraint

unique or primary key constraints on table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>developers_api_key_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_email_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_github_handle_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>developers_uid_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### developers_select_column

select columns of table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>active</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>api_key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>github_handle</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>onboarded</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uid</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### developers_update_column

update columns of table "developers"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>active</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>api_key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>email</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>github_handle</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>onboarded</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uid</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### end_user_conversations_constraint

unique or primary key constraints on table "end_user_conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>end_user_conversations_end_user_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_conversations_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### end_user_conversations_select_column

select columns of table "end_user_conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### end_user_conversations_update_column

update columns of table "end_user_conversations"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### end_users_constraint

unique or primary key constraints on table "end_users"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>end_users_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>end_users_uuid_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### end_users_select_column

select columns of table "end_users"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uuid</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### end_users_update_column

update columns of table "end_users"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_name</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>uuid</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### events_select_column

select columns of table "events"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>action</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>changed_fields</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>developer_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>table</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>timestamp</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### history_select_column

select columns of table "history"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>interval</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterances</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>window</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### kv_scope_enum_constraint

unique or primary key constraints on table "kv_scope_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>kv_scope_enum_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### kv_scope_enum_select_column

select columns of table "kv_scope_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### kv_scope_enum_update_column

update columns of table "kv_scope_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### kv_store_constraint

unique or primary key constraints on table "kv_store"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>kv_store_key_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>kv_store_object_id_key</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
<tr>
<td valign="top"><strong>kv_store_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### kv_store_select_column

select columns of table "kv_store"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_by</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### kv_store_update_column

update columns of table "kv_store"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>created_by</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>key</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>scope_object_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### last_utterance_select_column

select columns of table "last_utterance"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>interval</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>speaker_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>updated_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterance</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### objects_constraint

unique or primary key constraints on table "objects"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>objects_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### objects_select_column

select columns of table "objects"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### objects_update_column

update columns of table "objects"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>created_at</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>metadata</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>object_id</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### order_by

column ordering options

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>asc</strong></td>
<td>

in ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_first</strong></td>
<td>

in ascending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>asc_nulls_last</strong></td>
<td>

in ascending order, nulls last

</td>
</tr>
<tr>
<td valign="top"><strong>desc</strong></td>
<td>

in descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_first</strong></td>
<td>

in descending order, nulls first

</td>
</tr>
<tr>
<td valign="top"><strong>desc_nulls_last</strong></td>
<td>

in descending order, nulls last

</td>
</tr>
</tbody>
</table>

### speaker_type_enum_constraint

unique or primary key constraints on table "speaker_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>speaker_type_enum_pkey</strong></td>
<td>

unique or primary key constraint

</td>
</tr>
</tbody>
</table>

### speaker_type_enum_enum

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>bot</strong></td>
<td></td>
</tr>
<tr>
<td valign="top"><strong>user</strong></td>
<td></td>
</tr>
</tbody>
</table>

### speaker_type_enum_select_column

select columns of table "speaker_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### speaker_type_enum_update_column

update columns of table "speaker_type_enum"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>value</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

### utterances_select_column

select columns of table "utterances"

<table>
<thead>
<th align="left">Value</th>
<th align="left">Description</th>
</thead>
<tbody>
<tr>
<td valign="top"><strong>conversation_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>end_user_id</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>normalized_utterance</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>speaker_type</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>timestamp</strong></td>
<td>

column name

</td>
</tr>
<tr>
<td valign="top"><strong>utterance</strong></td>
<td>

column name

</td>
</tr>
</tbody>
</table>

## Scalars

### Boolean

The `Boolean` scalar type represents `true` or `false`.

### Float

The `Float` scalar type represents signed double-precision fractional values as specified by [IEEE 754](https://en.wikipedia.org/wiki/IEEE_floating_point).

### Int

The `Int` scalar type represents non-fractional signed whole numeric values. Int can represent values between -(2^31) and 2^31 - 1.

### JSON

The `JSON` scalar type represents JSON values as specified by [ECMA-404](http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-404.pdf).

### String

The `String` scalar type represents textual data, represented as UTF-8 character sequences. The String type is most often used by GraphQL to represent free-form human-readable text.

### _text

### app_status

### bigint

### inet

### jsonb

### numeric

### oid

### timestamptz

### tstzrange


## Interfaces


### Container

<table>
<thead>
<tr>
<th align="left">Field</th>
<th align="right">Argument</th>
<th align="left">Type</th>
<th align="left">Description</th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2" valign="top"><strong>has_vector</strong></td>
<td valign="top"><a href="#boolean">Boolean</a></td>
<td>

A boolean value indicating whether a word vector is associated with the object.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Verbatim text content.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>text_with_ws</strong></td>
<td valign="top"><a href="#string">String</a></td>
<td>

Text content, with trailing space character if present.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector</strong></td>
<td valign="top">[<a href="#float">Float</a>]</td>
<td>

A real-valued meaning representation.

</td>
</tr>
<tr>
<td colspan="2" valign="top"><strong>vector_norm</strong></td>
<td valign="top"><a href="#float">Float</a></td>
<td>

The L2 norm of the document’s vector representation.

</td>
</tr>
</tbody>
</table>

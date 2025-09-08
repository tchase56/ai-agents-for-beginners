<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "d2f04b783b9e1253100329afd698f8ff",
  "translation_date": "2025-08-29T23:30:37+00:00",
  "source_file": "05-agentic-rag/README.md",
  "language_code": "ja"
}
-->
[![Agentic RAG](../../../translated_images/lesson-5-thumbnail.20ba9d0c0ae64fae06637eb2023395d437b0152c0463c2227ff456afe5f14644.ja.png)](https://youtu.be/WcjAARvdL7I?si=BCgwjwFb2yCkEhR9)

> _(上の画像をクリックすると、このレッスンの動画をご覧いただけます)_

# エージェンティックRAG

このレッスンでは、エージェンティック・リトリーバル・オーグメンテッド・ジェネレーション（Agentic RAG）について包括的に解説します。これは、大規模言語モデル（LLM）が外部情報を取得しながら次のステップを自律的に計画するという、新たなAIパラダイムです。静的な「取得して読む」パターンとは異なり、エージェンティックRAGでは、ツールや関数の呼び出し、構造化された出力を挟みながら、LLMへの反復的な呼び出しが行われます。このシステムは結果を評価し、クエリを修正し、必要に応じて追加のツールを呼び出し、満足のいく解決策が得られるまでこのサイクルを続けます。

## はじめに

このレッスンでは以下を学びます：

- **エージェンティックRAGの理解：** LLMが外部データソースから情報を取得しながら次のステップを自律的に計画するという、新たなAIパラダイムについて学びます。
- **反復的なメイカー・チェッカースタイルの把握：** 正確性を向上させ、誤ったクエリを処理するために設計された、ツールや関数の呼び出し、構造化された出力を挟むLLMへの反復的な呼び出しのループを理解します。
- **実践的な応用の探求：** 正確性が重視される環境、複雑なデータベース操作、長期的なワークフローなど、エージェンティックRAGが活躍するシナリオを特定します。

## 学習目標

このレッスンを終えると、以下を理解し、実践できるようになります：

- **エージェンティックRAGの理解：** LLMが外部データソースから情報を取得しながら次のステップを自律的に計画するという、新たなAIパラダイムについて学びます。
- **反復的なメイカー・チェッカースタイル：** 正確性を向上させ、誤ったクエリを処理するために設計された、ツールや関数の呼び出し、構造化された出力を挟むLLMへの反復的な呼び出しのループを理解します。
- **推論プロセスの所有：** 問題へのアプローチ方法を事前定義されたパスに頼らず、自律的に決定するシステムの能力を理解します。
- **ワークフロー：** エージェンティックモデルが市場動向レポートを取得し、競合データを特定し、内部の販売指標を関連付け、結果を統合し、戦略を評価するプロセスを理解します。
- **反復ループ、ツール統合、メモリ：** 反復的なインタラクションパターンに依存し、ステップ間で状態とメモリを維持するシステムについて学びます。
- **失敗モードと自己修正の処理：** 診断ツールの使用や人間の監視に頼ることを含む、システムの堅牢な自己修正メカニズムを探ります。
- **エージェンシーの限界：** ドメイン固有の自律性、インフラ依存性、ガードレールの尊重に焦点を当てたエージェンティックRAGの限界を理解します。
- **実践的なユースケースと価値：** 正確性が重視される環境、複雑なデータベース操作、長期的なワークフローなど、エージェンティックRAGが活躍するシナリオを特定します。
- **ガバナンス、透明性、信頼：** 説明可能な推論、バイアス制御、人間の監視の重要性について学びます。

## エージェンティックRAGとは？

エージェンティック・リトリーバル・オーグメンテッド・ジェネレーション（Agentic RAG）は、大規模言語モデル（LLM）が外部情報を取得しながら次のステップを自律的に計画するという、新たなAIパラダイムです。静的な「取得して読む」パターンとは異なり、エージェンティックRAGでは、ツールや関数の呼び出し、構造化された出力を挟みながら、LLMへの反復的な呼び出しが行われます。このシステムは結果を評価し、クエリを修正し、必要に応じて追加のツールを呼び出し、満足のいく解決策が得られるまでこのサイクルを続けます。この反復的な「メイカー・チェッカー」スタイルは、正確性を向上させ、誤ったクエリを処理し、高品質な結果を保証します。

システムは推論プロセスを積極的に所有し、失敗したクエリを書き直し、異なる取得方法を選択し、複数のツール（Azure AI Searchのベクター検索、SQLデータベース、カスタムAPIなど）を統合して最終的な回答を出します。エージェンティックシステムの際立った特徴は、推論プロセスを自律的に所有する能力です。従来のRAG実装では事前定義されたパスに依存しますが、エージェンティックシステムは取得した情報の質に基づいてステップの順序を自律的に決定します。

## エージェンティックRAGの定義

エージェンティック・リトリーバル・オーグメンテッド・ジェネレーション（Agentic RAG）は、LLMが外部データソースから情報を取得するだけでなく、次のステップを自律的に計画するという、新たなAI開発のパラダイムです。静的な「取得して読む」パターンや慎重にスクリプト化されたプロンプトシーケンスとは異なり、エージェンティックRAGでは、ツールや関数の呼び出し、構造化された出力を挟むLLMへの反復的な呼び出しのループが含まれます。
<a href="https://learn.microsoft.com/training/modules/use-own-data-azure-openai" target="_blank">
Azure OpenAI Serviceを使用した検索強化生成（RAG）の実装: Azure OpenAI Serviceを使用して独自のデータを活用する方法を学びます。このMicrosoft Learnモジュールでは、RAGの実装に関する包括的なガイドを提供します。
- <a href="https://learn.microsoft.com/azure/ai-studio/concepts/evaluation-approach-gen-ai" target="_blank">Azure AI Foundryを使用した生成AIアプリケーションの評価: この記事では、Agentic AIアプリケーションやRAGアーキテクチャを含む、公開データセット上でのモデルの評価と比較について説明します。</a>
- <a href="https://weaviate.io/blog/what-is-agentic-rag" target="_blank">Agentic RAGとは | Weaviate</a>
- <a href="https://ragaboutit.com/agentic-rag-a-complete-guide-to-agent-based-retrieval-augmented-generation/" target="_blank">Agentic RAG: エージェントベースの検索強化生成に関する完全ガイド – RAGの最新情報</a>
- <a href="https://huggingface.co/learn/cookbook/agent_rag" target="_blank">Agentic RAG: クエリ再構築と自己クエリでRAGを強化！ Hugging FaceオープンソースAIクックブック</a>
- <a href="https://youtu.be/aQ4yQXeB1Ss?si=2HUqBzHoeB5tR04U" target="_blank">RAGにAgenticレイヤーを追加する</a>
- <a href="https://www.youtube.com/watch?v=zeAyuLc_f3Q&t=244s" target="_blank">知識アシスタントの未来: Jerry Liu</a>
- <a href="https://www.youtube.com/watch?v=AOSjiXP1jmQ" target="_blank">Agentic RAGシステムの構築方法</a>
- <a href="https://ignite.microsoft.com/sessions/BRK102?source=sessions" target="_blank">Azure AI Foundry Agent Serviceを使用してAIエージェントをスケールする</a>

### 学術論文

- <a href="https://arxiv.org/abs/2303.17651" target="_blank">2303.17651 Self-Refine: 自己フィードバックによる反復的な改良</a>
- <a href="https://arxiv.org/abs/2303.11366" target="_blank">2303.11366 Reflexion: 言語エージェントと言語強化学習</a>
- <a href="https://arxiv.org/abs/2305.11738" target="_blank">2305.11738 CRITIC: 大規模言語モデルはツールを活用した批評で自己修正が可能</a>
- <a href="https://arxiv.org/abs/2501.09136" target="_blank">2501.09136 Agentic Retrieval-Augmented Generation: Agentic RAGに関する調査</a>

## 前のレッスン

[ツール使用デザインパターン](../04-tool-use/README.md)

## 次のレッスン

[信頼できるAIエージェントの構築](../06-building-trustworthy-agents/README.md)

---

**免責事項**:  
この文書はAI翻訳サービス[Co-op Translator](https://github.com/Azure/co-op-translator)を使用して翻訳されています。正確性を追求しておりますが、自動翻訳には誤りや不正確な部分が含まれる可能性があります。元の言語で記載された文書を正式な情報源としてご参照ください。重要な情報については、専門の人間による翻訳を推奨します。この翻訳の使用に起因する誤解や誤解釈について、当方は一切の責任を負いません。
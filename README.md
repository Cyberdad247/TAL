
# TAL (Tree-structured Assembly Language)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15379276.svg)](https://zenodo.org/records/15379276)
[![Paper](https://img.shields.io/badge/PDF-TAL%20Paper-blue)](https://zenodo.org/records/15379276)

## 📖 概要 / Overview

「AIに命令するな。考え方を示せ。」  
"Don't command the AI. Show it how to think."

**TAL（Tree-structured Assembly Language）** は、大規模言語モデル（LLM）における**思考フレームワークを構造的に提示するプロンプト手法**です。  
TAL is a novel prompt methodology that presents structured thinking frameworks for Large Language Models (LLMs).

従来の命令型プロンプトではなく、**AIの推論プロセスそのものを明示的に設計**できるOS的インターフェースを目指しています。  
Instead of imperative commands, TAL serves as an OS-like interface to explicitly design the reasoning process of AI.

---

## 📚 ドキュメント一覧 / Documentation Index

- 📖 [TAL Blocks 解説書 (JP)](docs/TAL_blocks_jp.md)  
- 📖 [TAL Blocks Documentation (EN)](docs/TAL_blocks.md)  
- 🔁 [再帰構文設計ガイド (JP)](docs/Recursion_jp.md)  
- 🔁 [TAL Recursion Guide (EN)](docs/Recursion.md)  
- ⏩ [TALにおける並列処理 (JP)](docs/Parallel_Processing_in_TAL_jp.md)  
- ⏩ [Parallel Processing in TAL (EN)](docs/Parallel_Processing_in_TAL.md)  
- ❓ [FAQ（よくある質問）(JP)](docs/FAQ_jp.md)  
- ❓ [FAQ (EN)](docs/FAQ.md)
- 🤖 [TALによるシステム開発ガイド (JP)](docs/TALC_for_System_Manual_jp.md)
- 🤖 [System Development with TAL (EN)](docs/TALC_for_System_Manual.md)

---

## ✨ 特徴 / Features

1. **構造化された文法**により、AIに対して明確な思考フレームを提示可能。  
   Structured grammar offers clear cognitive frameworks to AI.

2. **TALコンパイラ** (**TALC**) を用いることで、複雑なTAL構文の記述・運用・変換を自動化できる。  
   With the TAL Compiler (TALC), you can automate the creation, transformation, and usage of TAL syntax.

3. **既存のプロンプト技術をTALでラッピング**することで、性能の底上げが可能となる。  
   Wrapping existing techniques (e.g., ToT, CoT, ReAct) within TAL enhances performance.

4. **TALブロックの再利用・組換え**により、目的別のプロンプトを柔軟に構築できる。  
   Reusable modular blocks allow flexible prompt construction tailored to different objectives.

5. 要約、対話、翻訳、創作など、**多様なAI活用領域にTALを適用可能**。  
   Applicable across tasks such as summarization, dialogue, translation, and creative generation.

6. 将来的には、**AIの深層制御や倫理的ガードレールの設計言語**としての拡張も期待される。  
   TAL is expected to become a language for deep control and ethical guardrail design in the future.

---

## 🤖 TALコンパイラ（TALC） / TAL Compiler (TALC)

ChatGPTのGPTsにて、TALC（TALコンパイラ）公開中！  
A public GPTs-based tool named TALC (TAL Compiler) is available here:  
➡️ [TALC](https://chatgpt.com/g/g-67f90502ff0c819199365f5bd3703e51-talc-tal-compiler)  

TALCを使えば、TALプロンプトを簡単に生成できます。  
またTALCは、TALについての疑問もその場で解決できる、対話型マニュアルとしても機能します！  
You can use TALC to generate TAL prompts easily, and also to ask questions about the TAL framework itself.  
It serves as both a prompt generator and an interactive guide to TAL's core concepts.  

---

## 📝 日本語論文 PDF / Japanese Paper

➡️ [TAL 日本語論文 PDF](https://raw.githubusercontent.com/tanep3/TAL/main/docs/tal_paper_jp.pdf)

---

## 🌐 英語版プレプリント / English Preprint

Zenodoにて英語版が公開されています：  
The English preprint is published on Zenodo:

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15379276.svg)](https://zenodo.org/records/15379276)

---

## 👤 著者 / Author

たねちゃんねるテクノロジー / Tane Channel Technology

➡️ [x.com/tanep3 (旧 Twitter)](https://x.com/tanep3)

---

## 💬 ディスカッション / Discussions

TALについての感想・活用事例・構文案・疑問など、なんでも気軽に話せる場所を開設しました。  
Discussions is open for your thoughts, feedback, ideas, and use-cases related to TAL.

🗣 こちらから参加できます！  
➡️ [GitHub Discussions](https://github.com/tanep3/TAL/discussions)

---

## 🙌 コントリビューション / Contributions

Issue・Pull Request歓迎です！質問や提案がある方もお気軽にどうぞ。  
構文の改善・追加・バグ修正・構文テンプレートの共有など、貢献も大歓迎です！  
Feel free to open issues or pull requests. Feedback and suggestions are welcome!  
We're happy to welcome contributions such as improvements, new syntax ideas, or bug fixes.  

✍️ Issue投稿やPRはこちら：  
➡️ [GitHub Issues](https://github.com/tanep3/TAL/issues)  
➡️ [Pull Requests](https://github.com/tanep3/TAL/pulls)  

---

## 📚 TALをもっと知りたい方へ / Learn More about TAL 

### 🌸 日本語ブログ（たねちゃんねるテクノロジー WEB版）  
📝 [Official Blog (JP)](https://tanep.work/tanech/)

TAL（Tree-structured Assembly Language）について、日本語で丁寧に解説しています。

---

### 🌍 English Article on Medium  
📝 [Medium (EN)](https://tanep3.medium.com/)

TAL is a prompt OS that gives AI structured thought instead of commands. This article introduces the idea in English with clear logic and practical examples.

---

## ⚖️ ライセンス / License

本プロジェクトは **CC BY 4.0（表示-継承）** ライセンスで公開されています。  
This project is licensed under **CC BY 4.0 (Attribution)**.  
➡️ https://creativecommons.org/licenses/by/4.0/
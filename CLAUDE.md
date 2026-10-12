# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 開発の進め方

- 実装を自律的に任せる前に、アーキテクチャ・issue の粒度・スコープを人間と議論して決める。決まっていない論点があれば、実装に入る前に挙げて確認する（先に任せすぎると、意図と違う方向に育って作り直しになる）

## 注意点

- 日本語でコミュニケーションする
- `.claude/skills/` の develop-issue / reflect-and-improve / improve-prompt / remove-ai-tells は [ha1f/news](https://github.com/ha1f/news) から移植したコピーで、元の版は news にある。クラウドの run は `~/.claude/skills/` を読まないため、この repo にも置いている。これらのスキル本体や LESSONS を変える PR には、news にも同じ反映が要るかを本文に書く（書かないと学びが片方の repo にだけ残る）
- 移植したファイルに出てくる issue / PR 番号と実測値は ha1f/news でのもの
- 自律開発ループ（GUARDRAILS.md・review-and-merge など）はまだ入れていない。develop-issue の保護パス確認（`check_protected_paths.py`）はこの repo では行わない

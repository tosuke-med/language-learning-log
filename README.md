---
layout: default
title: How to Use This Log / ログの使い方
permalink: /readme/
---

# language-learning-log

Language learning log with LLM — personal logs for English and French by a Japanese researcher.

The site is published at: **https://tosuke-med.github.io/language-learning-log/**

---

## How to add a new log entry / ログの追加方法

### File location / ファイルの場所

Place new log files under the appropriate directory:

- English logs: `content/en/logs/YYYY-MM-DD.md`
- French logs: `content/fr/logs/YYYY-MM-DD.md`

### Log template (writing practice) / ログのテンプレート（output練習用）

Use this template when practicing writing (output practice with phrase correction by LLM).  
このテンプレートはwritingなどのoutput練習で、LLMによるフレーズ修正を記録する際に使います。

```markdown
---
title: <topic title here>
date: YYYY-MM-DD
language: en
tags: [writing]
---

## Today's topic
<Topic in one line>

## Today's practice phrases
<List the phrases you want to practice or that you are unsure about, one per line.
 Intentional mistakes are fine — the LLM will correct them below.>

## Correction and explanation from LLM
<LLM-generated corrections and explanations in English go here.
 For each phrase: show the corrected version, then explain the grammar/usage point.>

## Comments
<Your own reflections in Japanese or English.>
```

**Front matter fields / フロントマターの項目:**

| Field | Description |
|-------|-------------|
| `title` | Short title for the log entry (shown on the site index) |
| `date` | Date in `YYYY-MM-DD` format |
| `language` | `en` or `fr` |
| `tags` | List of tags, e.g. `[writing]`, `[listening]`, `[reading]`, `[speaking]` |

### Asking the LLM for corrections / LLMへの修正依頼の仕方

After writing your practice phrases, ask the LLM:  
練習フレーズを書いたら、以下のように依頼してください：

> Please correct the practice phrases in the `## Today's practice phrases` section and fill in `## Correction and explanation from LLM` with corrections and explanations in English. The tag is `writing`.

Then paste the LLM output into the `## Correction and explanation from LLM` section, and add your own comments to `## Comments`.  
LLMの出力を`## Correction and explanation from LLM`に貼り付け、自分の感想を`## Comments`に書いてください。

---

## GitHub Pages

This site is built with Jekyll and published automatically via GitHub Pages from the `main` branch.

- Site URL: https://tosuke-med.github.io/language-learning-log/
- Theme: custom layout in `_layouts/default.html`
- Config: `_config.yml`

To publish a new entry, commit and push the new `.md` file to `main`. GitHub Pages will rebuild the site automatically.  
新しいエントリをmainにpushすると、GitHub Pagesが自動的にサイトを再ビルドします。

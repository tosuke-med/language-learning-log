---
title: Language Learning Logs with LLM
---

This site contains personal learning logs for English and French by a Japanese researcher.

I use large language models (LLMs) mainly as reflective tools:
to rewrite, summarize, and notice patterns — not to collect or memorize expressions.

From time to time, I summarize accumulated logs using LLMs
and write short notes or tips about how LLMs actually help (or don’t).

---

## English — Logs

{% assign en_logs = site.pages
  | where_exp: "p", "p.path contains 'content/en/logs/'"
  | where_exp: "p", "p.name != 'index.md'"
  | sort: "date"
  | reverse
%}

{% for p in en_logs %}
- {{ p.date | date: "%Y-%m-%d" }} — [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

## English — Summaries & LLM tips

{% assign en_syn = site.pages
  | where_exp: "p", "p.path contains 'content/en/synthesis/'"
  | where_exp: "p", "p.name != 'index.md'"
  | sort: "date"
  | reverse
%}

{% for p in en_syn %}
- {{ p.date | date: "%Y-%m-%d" }} — [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

## French — Logs

{% assign fr_logs = site.pages
  | where_exp: "p", "p.path contains 'content/fr/logs/'"
  | where_exp: "p", "p.name != 'index.md'"
  | sort: "date"
  | reverse
%}

{% for p in fr_logs %}
- {{ p.date | date: "%Y-%m-%d" }} — [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

---

## French — Summaries & LLM tips

{% assign fr_syn = site.pages
  | where_exp: "p", "p.path contains 'content/fr/synthesis/'"
  | where_exp: "p", "p.name != 'index.md'"
  | sort: "date"
  | reverse
%}

{% for p in fr_syn %}
- {{ p.date | date: "%Y-%m-%d" }} — [{{ p.title }}]({{ p.url | relative_url }})
{% endfor %}

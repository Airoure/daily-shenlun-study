# Source Configuration

Use this file as the configurable source list for daily Shenlun material collection. Prefer enabled sources. Add or disable sources only when the user asks to change the skill permanently.

## Selection Defaults

- Recency window: prefer last 30 days; expand to 90 days when needed.
- Daily item count: 3-5.
- Source mix: policy + commentary + grassroots case + data.
- Citation: cite every collected current item with title, publisher, date when available, and URL.
- Reliability: prefer official or primary pages over reposts.

## Enabled Sources

| id | enabled | type | name | url | use_for | query_hint |
|---|---|---|---|---|---|---|
| gov-policy-library | yes | policy | 国务院政策文件库 | https://sousuo.www.gov.cn/zcwjk/policyDocumentLibrary | 最新政策文件、政策关键词、治理主题 | site:gov.cn 国务院 政策 文件 最新 |
| gov-policy-interpretation | yes | policy_explainer | 中国政府网政策解读 | https://www.gov.cn/zhengce/jiedu/home.htm | 政策背景、目标、措施、解释逻辑 | site:gov.cn 政策解读 最新 |
| people-renmin-shiping | yes | commentary | 人民日报人民时评 | https://opinion.people.com.cn/GB/8213/353915/353916/index.html | 评论结构、规范表达、大作文立意 | site:opinion.people.com.cn 人民时评 最新 |
| banyuetan | yes | case_commentary | 半月谈 | https://www.banyuetan.org/ | 基层治理、民生痛点、形式主义、社会观察 | 半月谈 基层治理 最新 |
| stats | yes | data | 国家统计局 | https://www.stats.gov.cn/sj/ | 宏观数据、年度公报、民生和经济事实 | site:stats.gov.cn 最新 数据 统计公报 |
| moa-rural | yes | grassroots_case | 农业农村部乡村振兴/治理 | https://jhs.moa.gov.cn/xczx/ | 乡村振兴、乡村治理、案例做法 | site:moa.gov.cn 乡村振兴 典型案例 最新 |

## Source Role

Use `policy` items to identify direction and official wording.

Use `policy_explainer` items to understand "background -> problem -> measure -> target".

Use `commentary` items to learn argument structure and high-level expression.

Use `case_commentary` and `grassroots_case` items to build concrete material for point extraction, countermeasure writing, and example accumulation.

Use `data` items as evidence. Do not force data into every task if the theme does not need it.

## Search Pattern

When starting today's session, run searches like:

```text
<source query_hint> <current theme if known>
```

If there is no known theme, search broad current topics across the enabled source mix, then choose one theme with good policy + case support.

## Material Scoring

Score candidate material mentally before selecting it:

- 3 points: has a clear public problem or policy question.
- 2 points: has concrete measures, mechanisms, or cases.
- 2 points: has usable official wording.
- 2 points: has data or facts.
- 1 point: matches the learner's current weak point.

Prefer the highest-scoring theme. If two themes are close, pick the one better suited to today's weak point.

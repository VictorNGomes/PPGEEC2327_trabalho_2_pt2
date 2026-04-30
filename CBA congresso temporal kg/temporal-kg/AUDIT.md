# Temporal Knowledge Graph Audit

- Articles processed: 20
- Nodes: 314
- Edges: 659

## Node Counts
- Article: 20
- Author: 52
- Affiliation: 34
- Keyword: 141
- Theme: 63
- Year: 4

## Edge Counts
- Was_Author_of: 54
- Is_Linked_to: 117
- Contains: 141
- Was_Associated_To: 63
- Has_Expertise_In: 168
- Next_Time: 3
- Collaborates: 93
- Was_Published_In: 20

## Extraction Notes
- `1998/001.pdf`: missing_non_english_abstract, some_author_emails_missing_or_not_assignable
- `1998/002.pdf`: some_author_emails_missing_or_not_assignable
- `1998/351.pdf`: missing_non_english_abstract, missing_english_abstract, missing_keywords, missing_affiliations, some_author_emails_missing_or_not_assignable
- `1998/352.pdf`: missing_non_english_abstract, missing_english_abstract, author_affiliation_links_are_article_level, some_author_emails_missing_or_not_assignable
- `2000/162.pdf`: missing_non_english_abstract, missing_keywords
- `2000/164.pdf`: missing_non_english_abstract, missing_keywords
- `2000/CBA007.pdf`: some_author_emails_missing_or_not_assignable
- `2000/CBA623.pdf`: missing_non_english_abstract, author_affiliation_links_are_article_level, some_author_emails_missing_or_not_assignable
- `2000/CBA624.pdf`: missing_non_english_abstract, missing_english_abstract, some_author_emails_missing_or_not_assignable
- `2002/43.pdf`: missing_non_english_abstract
- `2002/48.pdf`: missing_english_abstract, author_affiliation_links_are_article_level
- `2002/874.pdf`: author_affiliation_links_are_article_level
- `2002/875.pdf`: author_affiliation_links_are_article_level
- `2002/877.pdf`: author_affiliation_links_are_article_level
- `2004/1323.pdf`: author_affiliation_links_are_article_level
- `2004/1325.pdf`: author_affiliation_links_are_article_level, some_author_emails_missing_or_not_assignable
- `2004/211.pdf`: author_affiliation_links_are_article_level
- `2004/212.pdf`: author_affiliation_links_are_article_level

## Modeling Notes
- `Collaborates` edges are stored once with `directed=false` in JSON/CSV; the GraphML export includes reciprocal directed edges for tools that do not support mixed directed and undirected edges.
- `Is_Linked_to` uses article-level affiliation evidence when the PDF layout does not unambiguously map each author to one institution.
- `Theme` nodes come from the prior graphify semantic extraction; `Keyword` nodes come from explicit keyword sections when readable.

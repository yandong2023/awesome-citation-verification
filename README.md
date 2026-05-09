# Awesome Citation Verification

[English](README.md) | [中文](README.zh-CN.md)

A practical guide to checking whether academic references are real, matched to the right paper, and defensible before you cite them.

This repository is for researchers, medical writers, students, reviewers, and editors who need to catch fake citations, hallucinated references, DOI mismatches, and weak source support before submission.

## Why this exists

AI writing tools can produce fluent text with references that look credible but fail basic checks:

- The DOI does not exist.
- The DOI exists but belongs to a different paper.
- The title, year, journal, or authors do not match.
- The paper is real but does not support the claim.
- The citation is copied from a review without checking the original source.

Citation verification is not just bibliography cleanup. It is a defensibility check: can you explain why this exact source supports this exact statement?

## Quick workflow

1. Extract every cited reference from the draft.
2. Check DOI existence and resolver behavior.
3. Match title, authors, year, journal, volume, issue, and pages.
4. Search PubMed, Crossref, OpenAlex, Semantic Scholar, or publisher pages.
5. Read the abstract or full text passage that is supposed to support the claim.
6. Mark each citation as `verified`, `needs review`, `mismatched`, `not found`, or `does not support claim`.
7. Replace weak or suspicious citations before submission.

## Useful resources in this repo

- [Check if a reference is real](checklists/check-if-a-reference-is-real.md)
- [Citation integrity report template](templates/citation-integrity-report.md)
- [Suspicious reference patterns](examples/suspicious-reference-patterns.md)

## Tools and databases to check citations

| Need | Useful places to check |
| --- | --- |
| DOI existence | Crossref, DOI.org, DataCite |
| Biomedical article metadata | PubMed, PubMed Central |
| Broad scholarly metadata | OpenAlex, Semantic Scholar |
| Publisher confirmation | Journal or publisher article page |
| Claim support | Abstract, full text, figures, tables, cited passages |

For a faster workflow, LitSource provides tools for citation checking and claim-to-source search:

- Citation checker: https://litsource.net/citation-checker?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification
- Reverse literature search: https://litsource.net/reverse-literature-search?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification
- ChatGPT fake references checker: https://litsource.net/chatgpt-fake-references-checker?utm_source=github&utm_medium=repo&utm_campaign=awesome-citation-verification

## What a good citation check should answer

- Does this reference exist?
- Does the DOI resolve to the same title?
- Do the authors, year, journal, and pages match?
- Is it indexed in a trusted database?
- Does the source actually support the sentence where it is cited?
- If it is uncertain, what should the writer do next?

## Status labels

Use simple labels when reviewing a bibliography:

| Status | Meaning |
| --- | --- |
| `verified` | Metadata matches and the source appears to support the cited statement. |
| `metadata mismatch` | The reference exists, but title, author, year, DOI, or journal details conflict. |
| `not found` | No reliable source record was found. |
| `suspicious` | The reference has signs of fabrication or copied metadata. |
| `does not support claim` | The article is real, but it does not support the statement being cited. |
| `needs manual review` | The automated or first-pass check is inconclusive. |

## Who should use this

- Medical writers checking references before client delivery.
- Graduate students cleaning AI-assisted drafts.
- Researchers preparing journal submissions.
- Editors checking suspicious bibliographies.
- Reviewers responding to unverifiable citations.

## Contributing

Pull requests are welcome for new checklists, examples, templates, and database-specific verification tips. Keep examples educational and avoid naming private individuals.

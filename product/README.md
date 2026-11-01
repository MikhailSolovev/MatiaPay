# MatiaPay — Product

Product management docs for MatiaPay: paying with your face. Code lives in [`../app`](../app); the *what* and *why* live here.

## Layout

| Folder | What goes here | Update when |
|---|---|---|
| [vision](vision/) | Product vision, target personas | Strategy shifts |
| [strategy](strategy/) | Market and competitor notes, OKRs | Every quarter |
| [discovery](discovery/) | Hypotheses and user-research notes | Before building anything new |
| [requirements](requirements/) | PRDs and user stories, one file per feature | Per feature |
| [roadmap](roadmap/) | Now / Next / Later roadmap | Monthly |
| [compliance](compliance/) | Biometric privacy, consent, fraud and payment-regulation risks | Before any release touching face data or payments |
| [metrics](metrics/) | North-star and product metric definitions | A metric is added or redefined |
| [decisions](decisions/) | Product decision log, one numbered file per decision | A non-obvious call is made |
| [releases](releases/) | Release notes | Every release |

## Conventions

- One feature = one PRD at `requirements/<feature-slug>.md`, copied from `prd-template.md`.
- Decisions are numbered `NNNN-short-title.md`, copied from `decisions/0000-template.md`. Accepted decisions are not edited; a new one supersedes them.
- The backlog lives in the issue tracker, not here. PRDs link to the issues.
- Every file starts as a template: replace `TBD` and the `<!-- hints -->` as you learn, delete sections that never apply.

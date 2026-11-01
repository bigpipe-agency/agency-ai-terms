# Agency AI policy data

Three open data files about how marketing agencies say they use AI, collected and coded by BigPipe in October and November 2026. The coding is free to reuse under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) with a credit to BigPipe; quoted words belong to each agency.

## agency-ai-policy-library-2026.csv

One row per AI policy that a marketing, PR, creative, web, SEO or social agency publishes about its own work: 68 policies, each read in full between October 25 and 30, 2026. A commitment is marked only when the policy states it as the agency's own practice (advice to others, templates and values without a practice behind them are not counted). The agency's exact wording for every marked commitment, and a page per policy, are in the [agency AI policy library](https://bigpipe.agency/agency-ai-policies).

| Column | Meaning |
| --- | --- |
| `agency` | Agency name as it appears on its site |
| `website` | The agency's domain, without www |
| `policy_url` | The page the policy was read on |
| `agency_type` | `marketing`, `pr`, `creative`, `web-digital`, `seo-content`, `social` or `production` |
| `country` | Where the agency is based when its site says so (`US`, `UK`, `AU`, `CA`, `NZ`, `DE`, `ZA`), blank otherwise |
| `format` | `policy page`, `blog post`, `PDF` or `section of a legal page` |
| `policy_date` | The date the page states for the policy, blank if it states none |
| `disclosure_timing` | When the agency tells clients about AI use: `proactive` (up front) or `on-request`, blank if the policy does not say |
| `disclosure_when` | When the disclosure applies, read from the agency's own words: `every` (whenever AI is used), `material` (when AI materially shapes a deliverable), `before` (raised with the client before AI is used), `standing` (one published statement of how AI runs through the work), `promise` (a general promise of openness naming no moment), `asked` (when the client asks); blank if the policy does not say it tells clients. Every statement, grouped this way: https://bigpipe.agency/ai-disclosure-statement-examples?utm_source=github&utm_medium=repo&utm_campaign=ai-terms&utm_content=research-readme |
| `humanReview` | `yes` if a person reviews, edits or approves AI-assisted work before the client sees it or it goes live |
| `disclosure` | `yes` if the agency tells clients how AI was used |
| `clientData` | `yes` if it sets a concrete rule on what client confidential or personal information may go into an AI tool |
| `limits` | `yes` if it names work it does not hand to AI (strategy, final creative, publishing, and the like) |
| `ipOriginality` | `yes` if it addresses copyright, ownership, originality checks, or consent for using a person's image or voice |
| `owner` | `yes` if it names the person, role or group accountable for how it uses AI |
| `clientControl` | `yes` if clients can limit or exclude AI on their work, or it follows the client's own AI rules |
| `namedTools` | `yes` if it names the AI tools it uses or has approved |
| `tools_named` | The tools named, separated by semicolons |
| `read_on` | The date the policy was read (policies change; re-read the original before relying on one) |

The live copy is at [bigpipe.agency/agency-ai-policies/library.csv](https://bigpipe.agency/agency-ai-policies/library.csv) and grows as policies are added.

## agency-ai-contract-clauses-2026.csv

One row per AI clause in an agency's own published client terms (terms of business, master services agreements, AI addenda): 99 clauses from 24 agencies in 10 countries, each document read in full on November 1, 2026. Only an agency's terms for its client work count (website terms of use, software terms and law-firm templates do not). Every clause, grouped by the question it settles, with each agency's document: https://bigpipe.agency/ai-contract-clauses?utm_source=github&utm_medium=repo&utm_campaign=ai-terms&utm_content=research-readme

| Column | Meaning |
| --- | --- |
| `agency` | Agency name |
| `document` | The document's own title |
| `document_url` | Where the document was read |
| `agency_type` | `marketing`, `creative`, `web-digital`, `seo-content` or `production` |
| `country` | Where the document or its address makes it clear (`US`, `UK`, `NZ`, `AU`, `DE`, `AT`, `NL`, `CA`, `JP`, `ZA`), blank otherwise |
| `document_date` | The date the document states for itself, blank if none |
| `clause_kind` | The question the clause settles: `use` (the agency uses AI), `transparency` (which AI, and where), `consent` (the client opts in, opts out or sets limits), `review` (human review of AI output), `data` (client data in AI tools and training), `ownership` (ownership and copyright of AI-made work), `warranty` (what the agency promises, disclaims or indemnifies), `tools` (third-party AI providers), `labeling` (labeling AI content for the public), `clientUse` (the client's own AI use), `pricing` (AI and the fee) |
| `clause_heading` | The clause number and heading as the document writes them |
| `clause_text` | The agency's exact words (spacing and line breaks normalized) |
| `read_on` | The date the document was read (contracts change; re-read the original before relying on one) |

The live copy is at [bigpipe.agency/ai-contract-clauses/clauses.csv](https://bigpipe.agency/ai-contract-clauses/clauses.csv).

## agency-ai-policy-audit-2026.csv

The counts from the October 19, 2026 audit of 104 small (2 to 10 person) US and UK client-service marketing agencies and the seven listed agency holding groups: how many mention AI on the homepage, sell it, say in writing how they use it, and publish an AI policy page. Columns: `measure`, `agencies` (count), `sample` (denominator), `share_pct`, `note`. Method, limits and references are in the [report](agency-ai-policy-audit-2026-report.pdf) ([Zenodo, DOI 10.5281/zenodo.23570587](https://doi.org/10.5281/zenodo.23570587)) and the summary in [agency-ai-policy-audit-2026-10.md](agency-ai-policy-audit-2026-10.md).

## Cite

BigPipe (2026). Agency AI Policy Audit 2026: How 104 small marketing agencies and seven holding groups disclose their use of AI. Zenodo. https://doi.org/10.5281/zenodo.23570587

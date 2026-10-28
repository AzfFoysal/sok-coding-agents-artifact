# Artifact: SoK: Security of AI Coding Agents in the Software Supply Chain

This repository holds the search, screening and coding records for the paper. Every count reported in the paper can be traced to a row in these files. The search and screening were completed on 27 October 2026.

## Files

### `SoK_literature_search_log.xlsx`: the complete review record

| Sheet | Contents |
|---|---|
| Protocol | Research questions, inclusion and exclusion criteria, the search string, the T7 scoping rule (protocol amendment), the screening and coding procedure, and the use of an LLM-based assistant. |
| Summary | Corpus totals: coded sources, academic vs. grey literature, peer-reviewed vs. preprint, threat-class counts, defense maturity (E0–E3), benchmarks. |
| Search Log | The 24 Phase 1 web-index queries, with dates, domain restrictions and result counts. |
| Database Search | The four Phase 2 runs in IEEE Xplore and the ACM Digital Library (main and delta strings, fields searched, date limits and hit counts; 766 hits in total). |
| DB Candidates | Database records selected for abstract screening. |
| Recall Check | The nine known records used to test the search string, and which string retrieved each. |
| Abstract Screening | All 165 abstract-screened database records, each with its decision and reason (coded, T7 aggregate, related work, excluded, duplicate, already in corpus). |
| Screening | All 49 Phase 1 records and the Phase 3 snowballing additions, each with its decision and reason. |
| Coding | The 96 coded primary sources: threat classes (primary and secondary), contribution type, attacker capability, SDLC stages, autonomy level, whether an agent was evaluated, defense enforcement point and maturity, and whether utility, adaptive attackers and artifacts are reported, with the evidence source and a full-text verification flag. |
| Double coding | The 17-paper reliability sample: first coding, the assistant's blind re-code (intra-coder check), the independent human coder's codes, and the Cohen's kappa computation for both comparisons. |

### `HumanCoder_packet_blank.xlsx`

The packet given to the independent human coder: instructions, codebook (T1–T8 definitions and decision rule), and the 17 sampled papers (title, venue, abstract) in random order (seed 7). It contains no earlier codes.

### `HumanCoder_packet_completed.xlsx`

The same packet as returned by the human coder, with a primary class, a confidence rating (1–3) and a note for each paper. These codes are column F of the Double coding sheet.

## Reliability

Agreement between the first coding and the independent human coder on primary threat class: 16 of 17 papers (p_o = 0.941, p_e = 0.211, Cohen's kappa = 0.93). The one disagreement was adjudicated as described in Section 3 of the paper.

## Notes

- Screening and first-pass coding were performed by an LLM-based research assistant applying the written criteria, with every decision reviewed by the author. Each decision is recorded with its reason so that it can be audited.
- 82 of the 96 coded sources were coded from abstracts and retrieved text; these are flagged in the Coding sheet for full-text verification.
- Counts describe the literature as of 27 October 2026.

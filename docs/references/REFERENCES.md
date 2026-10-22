# Reference papers

Primary sources for the algorithm in `PROJECT_SPEC.md` §5, by a link that does
not depend on a copy here. Only a copy licensed for redistribution is committed.

| Work | Identifier | Copy in this repository | Status |
|---|---|---|---|
| Weidner & Kleppmann, "The Art of the Fugue: Minimizing Interleaving in Collaborative Text Editing", *IEEE Transactions on Parallel and Distributed Systems* 36(11):2425–2437, November 2025. | DOI [10.1109/TPDS.2025.3611880](https://doi.org/10.1109/TPDS.2025.3611880). The authors' version: [arXiv:2305.00583v3](https://arxiv.org/abs/2305.00583v3), 21 October 2025. | none (removed, below) | **Normative for §5.** Defines FugueMax and proves maximal non-interleaving. |
| Weidner, Gentle & Kleppmann, "The Art of the Fugue: Minimizing Interleaving in Collaborative Text Editing", arXiv:2305.00583v1, 2023. 32pp. | [arXiv:2305.00583v1](https://arxiv.org/abs/2305.00583v1) | `fugue-arxiv-v1-extended-2023.pdf` | Supporting. Predates the FugueMax name but carries the full appendices: Appendix A worked anomaly examples, Appendix B impossibility proof for 3+ concurrent sites. Source for the fixed conformance traces (§9). |

Where the two disagree, the TPDS paper wins. Where the papers disagree with any
reference implementation, the papers win — and the disagreement gets recorded in
§13 rather than resolved silently.

**What "TPDS" means in a citation here.** The algorithm, line, figure,
definition and lemma numbers the spec, the code and the conformance traces cite
as TPDS were read from the copy committed for that purpose (§13.4), which was
arXiv v3 (below), not IEEE's typeset article. arXiv v3 is the freely reachable text
those numbers came from. Nobody here has compared it with the typeset version,
so a numbering difference found against the DOI copy is a §13 entry, not a typo.

## Removed: `fugue-tpds-2025.pdf`

Committed at `bdb7e94` (2026-09-01) and removed from the tree in the commit that
renamed this file from `README.md`. Despite its name it was not IEEE's copy: its
first page and its metadata identify it as arXiv:2305.00583v3, carrying arXiv's
non-exclusive distribution licence
(`http://arxiv.org/licenses/nonexclusive-distrib/1.0/`). That licence lets arXiv
distribute the paper and grants nobody else the right to, so serving it from a
public repository had no licence behind it, whichever version it was. **It
remains in history.** Why it stays there, and what removing it would cost, is
row 47 of the deferred register in `PROJECT_SPEC.md`.

## Kept: `fugue-arxiv-v1-extended-2023.pdf`

The v1 PDF's own metadata, set by the LIPIcs class the authors used, reads
"licensed under Creative Commons License CC-BY 4.0", which permits
redistribution with attribution; the citation above is that attribution. That is
the document's statement. arXiv's licence field for v1 was not reachable from
the environment that made this change, so it has not been checked against
arXiv's record.

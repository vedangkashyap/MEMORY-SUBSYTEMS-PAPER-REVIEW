# Cache Replacement Policy — Paper Reviews

Formal, one-page IEEE-format critical reviews of foundational and recent cache
replacement policy and TLB prefetching papers, written as part of independent
research work.

Each review follows a consistent structure:

1. **Introduction** — the specific gap in prior work the paper addresses
2. **Contribution** — what the paper concretely proposes
3. **Proposal** — the core mechanism, stated directly
4. **Key Results Achieved** — verified quantitative results from the paper
5. **Key Takeaway** — idea-level lessons, not a restatement of results
6. **Weakness** — specific limitations, grounded in the paper's own text and data
7. **Extension** — original, untried directions for future work

The goal of each review is not just to summarize the paper, but to critically
evaluate it and propose genuinely new extension ideas rather than simply citing
later work that addressed the same gap.

## Papers Reviewed

| Folder | Paper | Venue |
|---|---|---|
| [`rrip/`](./rrip) | A. Jaleel, K. B. Theobald, S. C. Steely Jr., J. Emer. "High Performance Cache Replacement Using Re-Reference Interval Prediction (RRIP)." | ISCA 2010 |
| [`ship/`](./ship) | C.-J. Wu, A. Jaleel, W. Hasenplaugh, M. Martonosi, S. C. Steely Jr., J. Emer. "SHiP: Signature-based Hit Predictor for High Performance Caching." | MICRO 2011 |
| [`daaip/`](./daaip) | Newton, S. K. Mahto, S. Pai, V. Singh. "DAAIP: Deadblock Aware Adaptive Insertion Policy for High Performance Caching." | ICCD 2017 |
| [`atp/`](./atp) | G. Vavouliotis, L. Alvarez, V. Karakostas, K. Nikas, N. Koziris, D. A. Jimenez, M. Casas. "Exploiting Page Table Locality for Agile TLB Prefetching." | ISCA 2021 |
| [`hawkeye/`](./hawkeye) | A. Jain, C. Lin. "Back to the Future: Leveraging Belady's Algorithm for Improved Cache Replacement." | ISCA 2016 |

Each folder contains:
- `review.tex` — LaTeX source (IEEE two-column format)
- `review.pdf` — compiled one-page review

## Note on Copyright

This repository contains only original review and analysis text written by the
author. It does **not** include copies of the original papers themselves, which
remain the copyright of their respective publishers (ACM / IEEE). Links to the
original papers can be found via their DOIs or publisher pages.

## Building from Source

Each `review.tex` uses the `IEEEtran` document class (two-column conference
format) and compiles with a standard LaTeX toolchain, e.g.:

```bash
pdflatex review.tex
```

Or paste the `.tex` contents directly into a new [Overleaf](https://www.overleaf.com)
project — `IEEEtran` is available by default there.

# Missing-count EM for capture-recapture

↑ **Parent:** [Capture-recapture model](capture-recapture-model.md)

Let $N_i=R_i-\sum_{s=i+1}^Jm_{is}$ count individuals never recaptured after release $i$. Partition them into death-interval counts $n_{ij}$ and terminal survivors $n_{iJ}$. Their unnormalized weights are $w_{ij}=(1-\phi_j)\prod_{\ell=i}^{j-1}\phi_\ell(1-P_{\ell+1})$ for $j<J$, and $w_{iJ}=\prod_{\ell=i}^{J-1}\phi_\ell(1-P_{\ell+1})$. Conditional counts are [multinomial](multinomial-distribution.md) with normalizer $C_i=\sum_{j=i}^Jw_{ij}$. The [EM algorithm](expectation-maximization-algorithm.md) replaces all missing counts by the displayed conditional expectations, then maximizes the resulting complete-data log likelihood. Survival and detection updates are expected successes divided by expected opportunities. A flat observed-likelihood ridge remains nonidentifiable even if each conditional complete-data maximization is explicit.

## ↑ Ancestors (8)

1. [Capture-recapture model](capture-recapture-model.md)
2. [Mark and recapture](mark-and-recapture.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/6/b/solution.md)

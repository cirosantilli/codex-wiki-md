# Biased cross-validation for density bandwidth

↑ **Parent:** [Cross-validation](cross-validation.md)

Subtract the diagonal variance contribution from the derivative estimate's squared norm, then insert the result into [asymptotic mean integrated squared error](asymptotic-mean-integrated-squared-error.md). The expected curvature estimate equals $R(f'')+O(h^2)$, apart from a negligible finite-n term. This makes the resulting criterion asymptotically correct even though it is not an exactly unbiased estimate of integrated risk. Under standard conditions its selector is ratio-consistent with the optimal bandwidth and has relative fluctuation order $n^{-1/10}$.

## ↑ Ancestors (8)

1. [Cross-validation](cross-validation.md)
2. [Statistical learning](statistical-learning-split.md)
3. [Statistical modelling](statistical-modelling-split.md)
4. [Statistical model](statistical-model-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

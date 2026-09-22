# Truncated singular value decomposition

↑ **Parent:** [Spectral regularization method](spectral-regularization-method.md)

For a [singular value decomposition](singular-value-decomposition.md) $A v_j=\sigma_j u_j$, truncated SVD with cutoff $\tau>0$ estimates the inverse action by $x_\tau=\sum_{\sigma_j\geq\tau}\sigma_j^{-1}\langle b,u_j\rangle v_j$. Discarding small singular values limits amplification of data errors; this is a [spectral regularization method](spectral-regularization-method.md).

Truncated singular value decomposition retains only singular components above a threshold, or equivalently only a finite leading set of singular vectors.

## ↑ Ancestors (7)

1. [Spectral regularization method](spectral-regularization-method.md)
2. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
3. [Inverse problem](inverse-problem-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

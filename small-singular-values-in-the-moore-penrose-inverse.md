# Small singular values in the Moore-Penrose inverse

↑ **Parent:** [Moore-Penrose inverse](moore-penrose-inverse.md)

For a nonzero [matrix](matrix.md) $A$, the [operator norm](operator-norm.md) induced by the [Euclidean norm](euclidean-norm.md) satisfies $\|A^+\|_2=1/\sigma_{\min,+}$, where $\sigma_{\min,+}$ is its smallest positive [singular value](singular-value.md). The [singular value decomposition](singular-value-decomposition.md) makes the danger visible: a small nonzero stretch becomes a large amplification of errors when inverted.

For instance, when $\varepsilon>0$,

$$
A_\varepsilon=\begin{pmatrix}1&0\\0&\varepsilon\end{pmatrix},
\qquad
A_\varepsilon^+=\begin{pmatrix}1&0\\0&1/\varepsilon\end{pmatrix}.
$$

A data perturbation $(0,\eta)^T$ changes the reconstructed input by $(0,\eta/\varepsilon)^T$. At $\varepsilon=0$, however, the [pseudoinverse](moore-penrose-inverse.md) is $\operatorname{diag}(1,0)$: exactly zero and merely small are different cases. Thus the [pseudoinverse](moore-penrose-inverse.md) need not be [continuous](continuous-function.md) across a change of [matrix rank](matrix-rank.md). With uncertain data, [truncated singular value decomposition](truncated-singular-value-decomposition.md) or [Tikhonov regularization](tikhonov-regularization.md) can trade exact inversion of weak directions for stability; the cutoff or penalty adds a modelling choice.

## ↑ Ancestors (7)

1. [Moore-Penrose inverse](moore-penrose-inverse.md)
2. [Matrix inverse](matrix-inverse.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

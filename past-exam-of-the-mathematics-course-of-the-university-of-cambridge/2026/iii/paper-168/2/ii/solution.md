<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Friedgut junta inequality](../../../../../../friedgut-junta-inequality.md) says that if $f:\{-1,1\}^n\to\{-1,1\}$ and

$$
\lVert f^{(\leq k)}\rVert_2^2\geq1-\varepsilon,
$$

then there is a real-valued $J$-[junta](../../../../../../junta.md) $g$ such that

$$
\lVert f-g\rVert_2^2\leq2\varepsilon,
\qquad
|J|\leq\frac{3^{2k}\mathbf I(f)^3}{\varepsilon^2}.
$$

To prove it, put $J=\{i:\operatorname{Inf}_i(f)\geq\tau\}$. Part (i), applied to each [discrete derivative of a Boolean function](../../../../../../discrete-derivative-of-a-boolean-function.md) $D_i f$, gives

$$
\sum_{i\notin J}\operatorname{Stab}_{1/3}(D_i f)
\leq\sum_{i\notin J}\lVert D_i f\rVert_{4/3}^2
=\sum_{i\notin J}\operatorname{Inf}_i(f)^{3/2}
\leq\tau^{1/2}\mathbf I(f).
$$

On the other hand, expanding the [noise stability](../../../../../../noise-stability.md) in [Fourier coefficients](../../../../../../fourier-walsh-transform.md) gives

$$
\sum_{i\notin J}\operatorname{Stab}_{1/3}(D_i f)
=3\sum_S|S\setminus J|3^{-|S|}\widehat f(S)^2
\geq3^{1-k}\sum_{\substack{S\not\subseteq J\\|S|\leq k}}\widehat f(S)^2.
$$

Choose $\tau=\varepsilon^2/(3^{2k}\mathbf I(f)^2)$ and define

$$
g=\sum_{\substack{S\subseteq J\\|S|\leq k}}\widehat f(S)\chi_S.
$$

The preceding bounds make the low-degree Fourier mass omitted by $g$ at most $\varepsilon$, while the hypothesis makes the high-degree mass at most $\varepsilon$. Thus $\lVert f-g\rVert_2^2\leq2\varepsilon$. Finally,

$$
|J|\tau\leq\sum_{i\in J}\operatorname{Inf}_i(f)\leq\mathbf I(f),
$$

which gives the asserted bound on $|J|$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

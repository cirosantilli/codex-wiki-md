<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Whenever the graded pieces $N_i$ are finitely generated over $S_0$, define the [Poincare series of a graded module](../../../../../../poincare-series-of-a-graded-module.md) by

$$
P_{N,\lambda}(t)=\sum_{i\ge0}\lambda(N_i)t^i.
$$

Additivity means $\lambda(B)=\lambda(A)+\lambda(C)$ for every [short exact sequence](../../../../../../short-exact-sequence.md) $0\to A\to B\to C\to0$ in the indicated category. Dimension over a [field](../../../../../../field.md) is a basic example; length is another when the [modules](../../../../../../module-mathematics.md) have finite length.

The [Hilbert-Serre theorem](../../../../../../hilbert-serre-theorem.md) needs finite-generation hypotheses: take $S_0$ commutative [Noetherian](../../../../../../noetherian-ring.md) and $S$ generated over it by homogeneous $x_1,\ldots,x_r$ of positive degrees $d_1,\ldots,d_r$. For finitely generated graded $N$, every $N_i$ is then finite over $S_0$, and

$$
\boxed{P_{N,\lambda}(t)=\frac{Q(t)}{\prod_{j=1}^r(1-t^{d_j})},\qquad Q(t)\in\mathbb Z[t]}.
$$

If negative grading indices are allowed for the [module](../../../../../../module-mathematics.md), the numerator is a [Laurent polynomial](../../../../../../laurent-polynomial.md) instead. In standard degree one, the coefficients are eventually [polynomial](../../../../../../polynomial-split.md) functions of the index.

To prove this, regard $N$ as finite over the surjective [polynomial](../../../../../../polynomial-split.md) presentation $S_0[X_1,\ldots,X_r]\to S$. Induct on $r$. At $r=0$ only finitely many homogeneous generator degrees occur, so the series is a [polynomial](../../../../../../polynomial-split.md). For the last variable $x$ of degree $d$, put $K=(0:_Nx)$ and $Q=N/xN$. The [polynomial ring](../../../../../../polynomial-ring.md) is [Noetherian](../../../../../../noetherian-ring.md) by the [Hilbert basis theorem](../../../../../../hilbert-basis-theorem.md), hence $K$ is finite; both $K$ and $Q$ are finite [modules](../../../../../../module-mathematics.md) over the [ring](../../../../../../ring.md) with that variable removed. The degree-$i$ exact sequence is

$$
0\longrightarrow K_{i-d}\longrightarrow N_{i-d}\xrightarrow{x}N_i\longrightarrow Q_i\longrightarrow0.
$$

Additivity, followed by summing over $i$, gives

$$
(1-t^d)P_{N,\lambda}=P_{Q,\lambda}-t^dP_{K,\lambda}.
$$

The induction hypothesis supplies the remaining denominator factors. This proves [Hilbert-Serre theorem for an additive coefficient function](../../../../../../hilbert-serre-theorem-for-an-additive-coefficient-function.md). If all $d_i=1$, expanding $(1-t)^{-r}$ proves eventual [polynomial](../../../../../../polynomial-split.md) coefficients directly.

An arbitrary positively [graded ring](../../../../../../graded-ring.md) in the introductory wording is not enough by itself. For example $S=k[X_1,X_2,\ldots]$ with every variable of degree one and $N=S$ is a cyclic [graded module](../../../../../../graded-module.md), but $N_1$ is not finite-dimensional over $k$, so the dimension-valued series is not even defined. The theorem above states the standard hypotheses that make the requested definition and rationality valid.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

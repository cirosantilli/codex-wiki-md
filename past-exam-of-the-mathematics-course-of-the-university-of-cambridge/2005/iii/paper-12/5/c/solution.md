<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The necessary and sufficient condition is

$$
\boxed{\sum_i p_i>0\quad\Longleftrightarrow\quad\rho(\Lambda)>1,}
$$

where $\rho$ is the [spectral radius](../../../../../../spectral-radius.md) of the [nonnegative matrix](../../../../../../nonnegative-matrix.md). No irreducibility is required. We use the given nonnegative-vector characterization of its Perron [eigenvalue](../../../../../../eigenvalue.md).

For necessity, suppose $p\ne0$ is the survival [fixed point](../../../../../../fixed-point.md) and let $S=\{i:p_i>0\}$. Since $1-e^{-z}<z$ for every $z>0$, its equation gives $(\Lambda p)_i>p_i$ for every $i\in S$. There are finitely many such coordinates, so

$$
\alpha=\min_{i\in S}\frac{(\Lambda p)_i}{p_i}>1.
$$

Outside $S$ the inequality $\Lambda p\ge\alpha p$ still holds, because its right side is zero and its left side is nonnegative. The provided [Perron–Frobenius theorem](../../../../../../perron-frobenius-theorem.md) characterization therefore gives $\rho(\Lambda)\ge\alpha>1$. In particular survival is impossible at $\rho=1$ for this Poisson offspring law.

Conversely suppose $\rho>1$. The given characterization supplies a nonzero $v\ge0$ with $\Lambda v\ge\rho v$; normalize it so $\max_i v_i=1$. For sufficiently small $\eta>0$,

$$
T_i(\eta v)\ge1-e^{-\eta\rho v_i}\ge\eta\rho v_i-\tfrac12\eta^2\rho^2v_i^2\ge\eta v_i.
$$

For example any $0<\eta\le\min(1,2(\rho-1)/\rho^2)$ works. Coordinates with $v_i=0$ satisfy the inequality automatically. Starting at $x_0=\eta v$, iterate $x_{t+1}=T(x_t)$. Monotonicity makes the sequence increase, and $T$ takes nonnegative [vectors](../../../../../../vector.md) into $[0,1]^l$, so it converges to a [fixed point](../../../../../../fixed-point.md) $x_\infty\ge\eta v\ne0$. Part (a) gives $p\ge x_\infty$, proving survival from at least one type. This proves the [spectral survival criterion for multitype Poisson branching](../../../../../../spectral-survival-criterion-for-multitype-poisson-branching.md) for reducible as well as irreducible reproduction [matrices](../../../../../../matrix.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

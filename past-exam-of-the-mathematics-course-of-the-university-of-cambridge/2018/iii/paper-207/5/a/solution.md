<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the event [counting process](../../../../../../counting-process.md) and [at-risk process](../../../../../../at-risk-process.md) by

$$
N_i(u)=v_i\mathbf1\{x_i\leq u\},\qquad Y_i(u)=\mathbf1\{x_i\geq u\},\qquad
N(u)=\sum_iN_i(u),\quad Y(u)=\sum_iY_i(u).
$$

Under a common [hazard function](../../../../../../hazard-function.md) and [independent censoring](../../../../../../independent-censoring.md), the conditional event rate is $Y(u)h(u)$. Equivalently, the [counting-process compensator](../../../../../../compensator-of-a-counting-process.md) satisfies $\mathbb E[dN(u)\mid\mathcal F_{u-}]=Y(u)dH(u)$. Estimate a [cumulative hazard](../../../../../../cumulative-hazard-function.md) increment by the observed event increment divided by the current [risk set](../../../../../../risk-set.md):

$$
d\widehat H(u)=\frac{dN(u)}{Y(u)}.
$$

With no ties, $dN$ has mass $v_i$ at $x_i$, and $Y(x_i)=\sum_{j:x_j\geq x_i}1$. Thus the [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) is

$$
\boxed{\widehat H(t)=\int_0^t\frac{dN(u)}{Y(u)}
=\sum_{i:x_i\leq t}\frac{v_i}{\sum_{j:x_j\geq x_i}1}.}
$$

Only event times contribute, so no empty [risk set](../../../../../../risk-set.md) is divided into an event count. [Right-censored](../../../../../../right-censoring.md) observations contribute time to the [risk sets](../../../../../../risk-set.md), but no event increment.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Risk-neutral valuation gives

$$
P_t^T
=\mathbb E^Q\left[
\prod_{s=t}^{T-1}(1+r_s)^{-1}
\,\middle|\,\mathcal F_t\right].
$$

For $s\geq t$,

$$
1+r_s=(1+r_t)\prod_{j=t}^{s-1}\zeta_j.
$$

Therefore

$$
\prod_{s=t}^{T-1}(1+r_s)^{-1}
=(1+r_t)^{-(T-t)}
\prod_{j=t}^{T-2}\zeta_j^{-(T-1-j)}.
$$

The future $\zeta_j$ are independent and identically distributed under the stated model, so

$$
\boxed{
P_t^T=(1+r_t)^{-(T-t)}
\prod_{k=1}^{T-t-1}M(-k),}
$$

with an empty product equal to one.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

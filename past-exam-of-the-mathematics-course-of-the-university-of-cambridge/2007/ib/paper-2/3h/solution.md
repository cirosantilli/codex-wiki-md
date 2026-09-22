<h1 id="3h/solution">Solution</h1>

↑ **Parent:** [3H](../3h.md)

Write $v_2(m)$ for the [2-adic valuation](../../../../../2-adic-valuation.md) of a nonzero integer $m$. Then $d(a,b)=2^{-v_2(a-b)}$ for unequal arguments. It is positive for $a\ne b$, vanishes exactly when $a=b$, and is symmetric because $v_2(-m)=v_2(m)$.

For the [triangle inequality](../../../../../triangle-inequality.md), if $2^r$ divides $a-b$ and $2^s$ divides $b-c$, then $2^{\min(r,s)}$ divides their sum $a-c$. Thus

$$
d(a,c)\le\max\{d(a,b),d(b,c)\}\le d(a,b)+d(b,c).
$$

Coincident arguments also satisfy these inequalities immediately. Consequently **$d$ is a [metric](../../../../../metric.md)**, and indeed an [ultrametric](../../../../../ultrametric.md) induced by the [2-adic absolute value](../../../../../2-adic-absolute-value.md).

For the sequence, $x_n-(-1)=2^n$, so

$$
\boxed{d(x_n,-1)=2^{-n}\longrightarrow0,\qquad x_n\longrightarrow-1.}
$$

The same sequence diverges in the usual Euclidean [metric](../../../../../metric.md); the convergence here depends on the [2-adic absolute value](../../../../../2-adic-absolute-value.md).

## ↑ Ancestors (10)

1. [3H](../3h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

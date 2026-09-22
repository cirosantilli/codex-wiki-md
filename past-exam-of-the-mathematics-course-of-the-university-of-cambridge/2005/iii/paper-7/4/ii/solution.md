<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $n\ge0$, put

$$
p_n(w)=\|f(w)^{2^n}\|^{1/2^n},\qquad M=\sup_{w\in\partial K}r(f(w)).
$$

The bound $r(u)\le\|u\|$ makes $M$ finite. Each $p_n$ is [continuous](../../../../../../continuous-function.md); [submultiplicativity](../../../../../../submultiplicativity.md) gives $p_{n+1}\le p_n$, and the [spectral radius formula](../../../../../../spectral-radius-formula.md) gives $p_n(w)\to r(f(w))$. [Spectral radius](../../../../../../spectral-radius.md) need not be [continuous](../../../../../../continuous-function.md), so applying the [Dini theorem](../../../../../../dini-s-theorem.md) directly to $p_n$ would not be justified. Instead define, on the [compact](../../../../../../compact-space.md) [boundary](../../../../../../boundary-of-a-set.md),

$$
q_n(w)=\max\{p_n(w),M\}.
$$

These are [continuous](../../../../../../continuous-function.md), decrease pointwise to the [continuous](../../../../../../continuous-function.md) constant $M$, and therefore converge uniformly by the [Dini theorem](../../../../../../dini-s-theorem.md). In particular,

$$
\limsup_{n\to\infty}\sup_{w\in\partial K}p_n(w)\le M.
$$

Multiplication is a [continuous](../../../../../../continuous-function.md) bilinear operation in a [Banach algebra](../../../../../../banach-algebra-split.md), so the [product rule](../../../../../../product-rule.md) shows that $w\mapsto f(w)^{2^n}$ is a [Banach-space-valued holomorphic function](../../../../../../banach-space-valued-holomorphic-function.md). Part (i), applied to this power, gives

$$
\|f(z)^{2^n}\|^{1/2^n}\le\sup_{w\in\partial K}\|f(w)^{2^n}\|^{1/2^n}.
$$

Taking the limit on the left and the limit superior on the right proves the [spectral-radius maximum principle](../../../../../../spectral-radius-maximum-principle.md):

$$
\boxed{r(f(z))\le\sup_{w\in\partial K}r(f(w)).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

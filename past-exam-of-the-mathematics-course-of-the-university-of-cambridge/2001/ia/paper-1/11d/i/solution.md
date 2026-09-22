<h1 id="11d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

By [continuity](../../../../../../continuous-function.md) of $g''$ at $\alpha$, for any $\epsilon>0$ choose $\delta(\epsilon)>0$ such that $|g''(s)|\le |g''(\alpha)|+\epsilon=:M$ whenever $|s-\alpha|<\delta(\epsilon)$. Twice using the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives the remainder as

$$
g(t)-g(\alpha)-g'(\alpha)(t-\alpha)=\int_\alpha^t[g'(s)-g'(\alpha)]\,ds.
$$

The inner difference is $\int_\alpha^s g''(r)\,dr$ and has modulus at most $M|s-\alpha|$. Integrating this bound over the interval between $\alpha$ and $t$ proves, for either sign of $t-\alpha$,

$$
\boxed{|g(t)-g(\alpha)-g'(\alpha)(t-\alpha)|\le L|t-\alpha|^2,\qquad L=(|g''(\alpha)|+\epsilon)/2.}
$$

This is the local quadratic [Taylor remainder](../../../../../../taylor-remainder.md) estimate. The given $\epsilon$ may enter the bound on the second derivative; no stronger differentiability assumption is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11D](../../11d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

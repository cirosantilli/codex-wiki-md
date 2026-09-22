<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $g\in L^2(\Omega)$, as required for the finite-valued data fidelity; extend the [total variation seminorm on a domain](../../../../../../total-variation-seminorm-on-a-domain.md) by $+\infty$ outside $BV(\Omega)$. The zero function is a finite-energy competitor. A minimizing sequence $f_n$ has bounded $\|f_n-g\|_2$ and bounded variation, hence bounded $L^2$ [norm](../../../../../../norm.md). Take a weakly convergent subsequence in $L^2$, with limit $f$. For each fixed test vector field $\zeta$, the pairing $\int f\operatorname{div}\zeta$ is weakly continuous because $\operatorname{div}\zeta\in L^2$. Its supremum has [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md). The squared [Hilbert space](../../../../../../hilbert-space-split.md) [norm](../../../../../../norm.md) also has [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md). Thus the [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md) gives a minimizer in $BV\cap L^2$.

The variation term is [convex](../../../../../../convex-function.md), and the squared fidelity term is [strictly convex](../../../../../../strictly-convex-function.md). Their sum is [strictly convex](../../../../../../strictly-convex-function.md) on its effective domain, so the minimizer is unique.

Let $T(t)=\min(b,\max(a,t))$. The [bounded-variation contraction under clipping](../../../../../../bounded-variation-contraction-under-clipping.md) gives $|D(T\circ f)|(\Omega)\le|Df|(\Omega)$. If $g(x)\in[a,b]$, then $|T(f(x))-g(x)|\le|f(x)-g(x)|$, strictly whenever $f(x)\notin[a,b]$. A positive-measure set outside the interval would therefore strictly decrease the fidelity integral, while not increasing variation, contradicting minimality. Hence

$$
\boxed{\text{a unique }f_*\in BV(\Omega)\cap L^2(\Omega)\text{ exists, and }a\le f_*\le b\text{ a.e.}}
$$

No compactness theorem for the $BV$ embedding is required for this weak-$L^2$ argument.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

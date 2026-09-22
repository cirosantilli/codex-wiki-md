<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First work at the level of [differential forms](../../../../../../differential-form-split.md). The fiber description implies $\pi\circ f=\pi$, so every pullback $\pi^*\beta$ is $f$-invariant. Since $\pi$ is a [surjective](../../../../../../surjective-function.md) [local diffeomorphism](../../../../../../local-diffeomorphism.md), its pullback on forms is [injective](../../../../../../injective-function.md): at any $y\in N$, choose a lift $x$ and use the inverse of $d\pi_x$ to evaluate the form on arbitrary tangent vectors at $y$.

Conversely let $\alpha$ be an $f$-invariant form on $M$. For a local inverse $s:V\to M$ of $\pi$, define $\beta|_V=s^*\alpha$. If two inverses select the same lift they agree locally; if they select different lifts, the fiber condition identifies the second with $f$ composed with the first. Locally these alternatives are stable, using disjoint inverse neighborhoods at distinct lifts. The equality $f^*\alpha=\alpha$ therefore makes the local definitions agree. They glue to a unique smooth form $\beta$ on $N$ with $\pi^*\beta=\alpha$. Thus

$$
\pi^*:\Omega^p(N)\cong\Omega^p(M)^f
$$

is an isomorphism of complexes, with the [exterior derivative](../../../../../../exterior-derivative.md) on both sides.

It remains to compare the [cohomology](../../../../../../cohomology-split.md) of the invariant complex with invariant [de Rham cohomology](../../../../../../de-rham-cohomology.md) classes. Put $P=(I+f^*)/2$ on forms. If $f^*[\alpha]=[\alpha]$ and $d\alpha=0$, then $P\alpha$ is invariant, closed and represents the same class, because its class is the average of two equal classes. If an invariant form is exact, $\alpha=d\eta$, then $\alpha=d(P\eta)$ with an invariant primitive. This proves both surjectivity and injectivity on [cohomology](../../../../../../cohomology-split.md). For $p=0$ there are no negative-degree primitives, and the same conclusion follows directly from closed functions.

Combining the two steps gives

$$
\boxed{\pi^*:H^p_{\mathrm{dR}}(N)\xrightarrow{\ \cong\ }H^p_+(M).}
$$

This is the [de Rham cohomology of a finite quotient](../../../../../../de-rham-cohomology-of-a-finite-quotient.md) argument specialized to an involution. It does not require [orientation](../../../../../../orientation-of-a-simplex.md). The hypotheses do not explicitly exclude $f=\operatorname{id}$; then all fibers are singletons, $\pi$ is a bijective [local diffeomorphism](../../../../../../local-diffeomorphism.md) and the conclusion is the ordinary [diffeomorphism](../../../../../../diffeomorphism.md) invariance. If $f$ has one fixed point, local injectivity of $\pi$ makes its fixed set open as well as closed; connectedness of $M$ forces this identity case. Otherwise the fibers have two points and $\pi$ is the usual double covering.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

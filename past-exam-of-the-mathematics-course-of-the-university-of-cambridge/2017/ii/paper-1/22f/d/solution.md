<h1 id="22f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $q$ be conjugate to $p$, so $1/q=1-1/p$, including $q=1$ for $p=\infty$. [Hölder's inequality](../../../../../../holder-s-inequality.md) implies, for every measurable finite-measure [set](../../../../../../set-split.md) $E$,

$$
\int_E|f_n|\,d\lambda\le M\lambda(E)^{1/q},\qquad
\int_E|f|\,d\lambda\le M\lambda(E)^{1/q}.
$$

This proves integrability on $A$ and gives [uniform integrability](../../../../../../uniform-integrability.md) there. Choose a [set](../../../../../../set-split.md) $B\subseteq A$ with $\lambda(A\setminus B)\le\delta$ on which convergence is uniform, using [Egorov theorem](../../../../../../egorov-s-theorem.md). Then

$$
\int_A|f_n-f|\,d\lambda
\le\lambda(A)\sup_B|f_n-f|+2M\delta^{1/q}.
$$

First take $n\to\infty$ and then $\delta\downarrow0$. Thus even the local $L^1$ difference tends to zero, and in particular

$$
\boxed{\int_A f_n\,d\lambda\longrightarrow\int_A f\,d\lambda}.
$$

For $1<p<\infty$, simple [functions](../../../../../../function-split.md) supported on finite-measure [Borel sets](../../../../../../borel-set.md) are dense in $L^q(\mathbb R)$. The displayed convergence proves pairing convergence for such [functions](../../../../../../function-split.md). Approximate any $h\in L^q$ by a simple $h_0$ and use

$$
\left|\int(f_n-f)(h-h_0)\,d\lambda\right|\le2M\|h-h_0\|_q.
$$

By the [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md), these are all [continuous linear functionals](../../../../../../continuous-linear-functional.md) on $L^p$, so $f_n$ converges weakly to $f$. It need not converge strongly: $f_n=\mathbf1_{[n,n+1]}$ converges pointwise to zero but has $L^p$ [norm](../../../../../../norm.md) one. For $p=\infty$ the pairing argument gives weak-star convergence against $L^1$, rather than asserting [weak convergence](../../../../../../weak-convergence.md) against every functional in the much larger full dual.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the bounded set $\Omega$ is measurable, as needed to define its indicator in $L^q$. Put $w_j=f_j-f$ and choose a smooth [cutoff function](../../../../../../cutoff-function.md) $\eta$ of compact support equal to one near $\Omega$. [Weak convergence](../../../../../../weak-convergence.md) in the [H1 space](../../../../../../h1-space.md) gives a uniform $H^1$ bound, by the [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md), and therefore $u_j=\eta w_j$ is uniformly bounded in $H^1$ with fixed compact support.

Here is a direct Fourier proof of the local compactness in the [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md). For each frequency $\xi$, $\widehat u_j(\xi)\to0$, since integrating $w_j$ against the fixed compactly supported function $\eta(x)e^{-ix\cdot\xi}$ is a continuous linear functional on $H^1$. Also $|\widehat u_j(\xi)|\leq C$ uniformly, by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) on the fixed support. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives, for every fixed $R$,

$$
\int_{|\xi|\leq R}|\widehat u_j(\xi)|^2\,d\xi\longrightarrow0.
$$

The uniform derivative bound and the unitary [Plancherel theorem](../../../../../../plancherel-theorem.md) control high frequencies:

$$
\int_{|\xi|>R}|\widehat u_j(\xi)|^2\,d\xi
\leq R^{-2}\int|\xi|^2|\widehat u_j(\xi)|^2\,d\xi
=R^{-2}\|\nabla u_j\|_2^2\leq C R^{-2}.
$$

First let $j\to\infty$, then $R\to\infty$. This proves $\|u_j\|_2\to0$, and hence $\|\chi_\Omega w_j\|_2\to0$.

Let $2^*=2n/(n-2)$. The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) bounds $\|u_j\|_{2^*}$ uniformly. For $2<q<2^*$, choose $\theta\in(0,1)$ with $1/q=\theta/2+(1-\theta)/2^*$. [Interpolation of Lp norms](../../../../../../lp-interpolation-inequality.md) gives $\|u_j\|_q\leq\|u_j\|_2^\theta\|u_j\|_{2^*}^{1-\theta}\to0$. For $1\leq q<2$, [Holder inequality](../../../../../../holder-inequality.md) on the fixed finite-measure support gives the same conclusion from $L^2$ convergence. Thus

$$
\boxed{\chi_\Omega f_j\longrightarrow\chi_\Omega f
\quad\text{strongly in }L^q,\qquad1\leq q<\frac{2n}{n-2}.}
$$

The same integral estimate covers $0<q<1$ if those spaces are interpreted with their usual quasi-norm. No conclusion at the critical exponent is asserted.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [normal family](../../../../../normal-family.md) of [holomorphic functions](../../../../../holomorphic-function.md) on a domain is one from which every sequence has a subsequence converging locally uniformly to a [holomorphic function](../../../../../holomorphic-function.md), or locally uniformly to infinity in the extended convention. For a bounded family, only finite limits occur.

For functions mapping a plane domain $D$ into the [unit disc](../../../../../unit-disc.md), the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) supplies uniform derivative bounds on each compact subset. More explicitly, if a closed disc of radius $r$ around $z$ lies in $D$, the [Cauchy estimate](../../../../../cauchy-estimate.md) gives $|f'(z)|\leq1/r$. A slightly larger compact neighborhood of any given compact set therefore gives uniform boundedness and equicontinuity there. Apply the [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md) on a compact exhaustion and take a diagonal subsequence. Its limit is locally uniform; the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) shows that the limit is [holomorphic](../../../../../complex-differentiability-at-a-point.md). This proves normality rather than merely invoking it.

Now let $|g|\leq M$ on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Every dilation $g_t(w)=g(tw)$ has the same bound, so the argument just given, after scaling the bound if necessary, proves that $\{g_t:t\geq1\}$ is a [normal family](../../../../../normal-family.md). For any sequence $t_j\to\infty$, every locally uniform subsequential limit $G$ satisfies

$$
G(iy)=\lim_jg(it_jy)=\ell\qquad(y>0).
$$

The [identity theorem for holomorphic functions](../../../../../identity-theorem.md) forces $G\equiv\ell$. It follows that $g_t\to\ell$ locally uniformly as $t\to\infty$: otherwise a sequence violating convergence on one compact set would have a convergent subsequence with this same constant limit, a contradiction.

For $0<\varepsilon<\pi/2$, the arc $K_\varepsilon=\{e^{i\theta}:\varepsilon\leq\theta\leq\pi-\varepsilon\}$ is a compact subset of the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Write $z=|z|w$ with $w\in K_\varepsilon$. Local uniform convergence of the dilations gives

$$
\boxed{g(z)\longrightarrow\ell\quad\text{as }|z|\to\infty\text{ in }S(\varepsilon).}
$$

For $\varepsilon\geq\pi/2$ the specified sector is empty. This is the same compactness mechanism as the [normal-family proof of angular boundary convergence](../../../../../normal-family-proof-of-angular-boundary-convergence.md).

To transfer the result to the [unit disc](../../../../../unit-disc.md), use the [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md)

$$
w=C_\omega(z)=i\frac{1+\overline\omega z}{1-\overline\omega z},\qquad
g(w)=h\left(\omega\frac{w-i}{w+i}\right).
$$

It sends $r\omega$ to $iy$ with $y=(1+r)/(1-r)$, so $g(iy)\to\ell$ as $y\to\infty$. Choose the curvature-minus-one normalization of the [hyperbolic metric](../../../../../hyperbolic-metric.md), for which the disc line element is $2|dz|/(1-|z|^2)$ and the half-plane line element is $|dw|/\operatorname{Im}w$. The [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md) preserves these metrics. For $w\in\mathbb H$ and $y>0$,

$$
\cosh\rho_{\mathbb H}(w,iy)
=\frac{|w|^2+y^2}{2y\operatorname{Im}w}
\geq\frac{|w|}{\operatorname{Im}w}.
$$

Thus $\rho_{\mathbb D}(z,r\omega)<k$ implies $\operatorname{Im}w/|w|>\operatorname{sech}k$. This is the [hyperbolic tube around a radial segment](../../../../../hyperbolic-tube-around-a-radial-segment.md) estimate. It places $w$ in a fixed sector bounded away from the real axis. Moreover $z\to\omega$ implies $|C_\omega(z)|\to\infty$. Applying the sector result gives

$$
\boxed{h(z)\longrightarrow\ell\quad\text{as }z\to\omega\text{ within }\Sigma(k).}
$$

A different constant normalization of the [hyperbolic metric](../../../../../hyperbolic-metric.md) only rescales $k$ and gives the same conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

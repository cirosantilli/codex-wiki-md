<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

As usual, the bounded set is assumed Lebesgue measurable and an $L^q$ exponent is positive; the conventional Banach-space assertion concerns $1\leq q<2^*=2n/(n-2)$. No boundary regularity of $\Omega$ is needed. Choose a smooth compactly supported cutoff $\eta$ equal to one on a ball containing $\Omega$. [Weak convergence](../../../../../../weak-convergence.md) and the [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) give a common $H^1$ bound for $f_j$, hence also for $g_j=\eta f_j$. These functions have a common compact support.

We prove their local $L^2$ compactness directly. Translation and the fundamental theorem along line segments give, by density from smooth functions,

$$
\|g_j(\cdot-h)-g_j\|_2\leq |h|\|\nabla g_j\|_2.
$$

For a compactly supported [mollifier](../../../../../../mollifier.md) $\rho_\varepsilon$, integration of this estimate gives

$$
\|g_j*\rho_\varepsilon-g_j\|_2\leq C\varepsilon\|\nabla g_j\|_2\leq C'\varepsilon.
$$

At fixed $\varepsilon$, [Hölder's inequality](../../../../../../holder-s-inequality.md) bounds $\|g_j*\rho_\varepsilon\|_\infty$ and $\|\nabla(g_j*\rho_\varepsilon)\|_\infty$ uniformly by the $L^2$ [norm](../../../../../../norm.md) of the corresponding smoothing kernels. Their supports lie in one fixed compact set, so the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) makes this smoothed family precompact in $L^2$. The uniform $O(\varepsilon)$ approximation makes the original family totally bounded in $L^2$: choose a finite net for the smoothed family and add the approximation error. Completeness gives relative compactness.

Every strongly convergent subsequence of $g_j$ has limit $\eta f$, since multiplication by $\eta$ preserves weak $L^2$ convergence. Consequently the whole sequence converges strongly: otherwise a subsequence with distance at least a fixed positive number would have a further convergent subsequence and contradict that unique limit. In particular $\|\chi_\Omega(f_j-f)\|_2\to0$.

The critical [Sobolev inequality](../../../../../../sobolev-inequality.md) supplies a uniform bound in $L^{2^*}$. For clarity, this estimate follows from part 2(a), not from compactness at the critical exponent. For a compactly supported smooth $v$, integrating by parts against the vector field $(x-y)/|x-y|^n$ gives

$$
|v(x)|\leq C_n\int |x-y|^{1-n}|\nabla v(y)|\,dy.
$$

Its distributional divergence is the sphere-area multiple of a point mass; applying the [Hardy–Littlewood–Sobolev inequality](../../../../../../hardy-littlewood-sobolev-inequality.md) with $\alpha=1,p=2$ yields $\|v\|_{2^*}\leq C\|\nabla v\|_2$. Density extends this to $H^1(\mathbb R^n)$.

For $2<q<2^*$ choose $0<\theta<1$ with $1/q=\theta/2+(1-\theta)/2^*$. [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\|\chi_\Omega(f_j-f)\|_q\leq\|\chi_\Omega(f_j-f)\|_2^\theta\|\chi_\Omega(f_j-f)\|_{2^*}^{1-\theta}\longrightarrow0.
$$

For $1\leq q<2$, use $\|v\|_{L^q(\Omega)}\leq|\Omega|^{1/q-1/2}\|v\|_{L^2(\Omega)}$. The same integral estimate also works for $0<q<1$ if $L^q$ is understood with its usual quasi-[norm](../../../../../../norm.md). Thus **$\chi_\Omega f_j\to\chi_\Omega f$ strongly for every positive $q<2^*$**. We have never asserted that multiplying by the possibly nonsmooth indicator preserves $H^1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

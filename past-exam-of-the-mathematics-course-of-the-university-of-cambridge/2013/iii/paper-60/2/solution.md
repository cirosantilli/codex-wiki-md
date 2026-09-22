<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Malgrange–Ehrenpreis theorem](../../../../../malgrange-ehrenpreis-theorem.md) states that **every nonzero constant-coefficient linear differential operator on [Euclidean space](../../../../../euclidean-norm.md) has a distributional fundamental solution**. With $D_j=\partial_{x_j}$ and $P(D)=\sum_{|\alpha|\leq N}a_\alpha D^\alpha$, the conclusion is an $E\in\mathcal D'(\mathbb R^d)$ such that $P(D)E=\delta_0$. If $N=0$, simply take $E=a_0^{-1}\delta_0$; hence assume $N\geq1$.

We construct a [Hörmander staircase](../../../../../hormander-staircase.md) in frequency space. The highest-degree homogeneous part $P_N$ is not identically zero on real vectors, since a [polynomial](../../../../../polynomial-split.md) vanishing on all real vectors has all coefficients zero. After an [orthogonal transformation](../../../../../orthogonal-transformation.md) of coordinates, we can arrange that $P_N(e_1)\ne0$. Thus, for each real $\xi'\in\mathbb R^{d-1}$, the [polynomial](../../../../../polynomial-split.md)

$$
p(z,\xi')=P(iz,i\xi')
$$

has degree $N$ in $z$ and the same nonzero leading coefficient $b=i^NP_N(e_1)$, independent of $\xi'$. This constant [leading coefficient of a polynomial](../../../../../leading-coefficient-of-a-polynomial.md) is what makes a uniform staircase possible.

For a fixed $\xi'$, factor $p(z,\xi')=b\prod_{\nu=1}^N(z-z_\nu)$, counting repeated [roots of a polynomial](../../../../../root-of-a-polynomial.md). Consider the $N+1$ heights $h_j=3j$, $j=0,\ldots,N$. A given root has imaginary part within distance less than one of at most one of these heights. By the [pigeonhole principle](../../../../../pigeonhole-principle.md), some height avoids every root, and then

$$
|p(s+ih_j,\xi')|=|b|\prod_\nu|s+ih_j-z_\nu|\geq|b|\qquad(s\in\mathbb R).
$$

This is [finite-height polynomial root avoidance](../../../../../finite-height-polynomial-root-avoidance.md). Root labels need not be chosen continuously or even measurably. Instead define the closed sets

$$
B_j=\bigcap_{q\in\mathbb Q}\{\xi':|p(q+ih_j,\xi')|\geq|b|\},\qquad
A_j=B_j\setminus\bigcup_{\ell<j}B_\ell.
$$

Continuity in $s$ extends the inequality from rational $q$ to every real $s$. These [Borel sets](../../../../../borel-set.md) partition $\mathbb R^{d-1}$. The [Hörmander staircase](../../../../../hormander-staircase.md) assigns the horizontal contour $s+ih_j$ over $A_j$; its height is bounded by $3N$, and the denominator has the uniform lower bound $|b|$. For $d=1$, the transverse space is a single point and only one horizontal contour is needed.

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat\varphi(\zeta)=\int e^{-ix\cdot\zeta}\varphi(x)\,dx$, with inverse factor $(2\pi)^{-d}$. Define the candidate [fundamental solution of a linear differential operator](../../../../../fundamental-solution-of-a-linear-differential-operator.md) by

$$
\langle E,\varphi\rangle=\frac1{(2\pi)^d}\sum_{j=0}^N\int_{A_j}\int_{\mathbb R}
\frac{\widehat\varphi(-s-ih_j,-\xi')}{P(i(s+ih_j),i\xi')}\,ds\,d\xi'.
$$

For a [test function](../../../../../test-function.md) supported in a fixed [compact set](../../../../../compact-space.md) $K$, [Fourier decay in a bounded complex strip](../../../../../fourier-decay-in-a-bounded-complex-strip.md) gives, for any integer $M$,

$$
|\widehat\varphi(-\xi-ih_je_1)|\leq C_{K,M,N}(1+|\xi|^2)^{-M}
\max_{|\alpha|\leq2M}\|D^\alpha\varphi\|_\infty.
$$

Indeed, this is the real [Fourier transform](../../../../../fourier-transform.md) of $e^{-h_jx_1}\varphi(x)$ with reversed frequency, and repeated [integration by parts](../../../../../integration-by-parts.md) with $(1-\Delta)^M$ proves the estimate. Taking $2M>d$ and using the denominator bound proves absolute convergence and a continuity estimate on $\mathcal D_K$. Thus $E$ is a [distribution](../../../../../distribution-mathematical-analysis.md); no unsupported interpretation of a divergent inverse [Fourier transform](../../../../../fourier-transform.md) is being used.

For its [distributional derivatives](../../../../../distributional-derivative.md), the [formal transpose of a differential operator](../../../../../formal-transpose-of-a-differential-operator.md) is $P(-D)$. Since

$$
\widehat{P(-D)\varphi}(-\zeta)=P(i\zeta)\widehat\varphi(-\zeta),
$$

applying $P(D)$ cancels the denominator. For each fixed $\xi'$, the numerator is an [entire function](../../../../../entire-function.md) of $z$. The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md), applied to a rectangle between the lines $\operatorname{Im}z=0$ and $\operatorname{Im}z=h_j$, gives

$$
\int_{\mathbb R}\widehat\varphi(-s-ih_j,-\xi')\,ds
=\int_{\mathbb R}\widehat\varphi(-s,-\xi')\,ds.
$$

The two vertical edges tend to zero by the same bounded-strip decay. The resulting [contour deformation](../../../../../contour-deformation.md) is performed separately for each transverse frequency, so discontinuities of the staircase height introduce no additional boundary terms. Absolute convergence permits integration over the partition $A_j$. The [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) then yields

$$
\boxed{\langle P(D)E,\varphi\rangle=\frac1{(2\pi)^d}\int_{\mathbb R^d}\widehat\varphi(-\xi)\,d\xi=\varphi(0).}
$$

This proves the [Malgrange–Ehrenpreis theorem](../../../../../malgrange-ehrenpreis-theorem.md). Undoing the orthogonal change of coordinates gives the [fundamental solution of a linear differential operator](../../../../../fundamental-solution-of-a-linear-differential-operator.md) for the original operator; the [Dirac delta distribution](../../../../../dirac-delta-function.md) is unchanged by that change of coordinates.

For a one-dimensional operator $L=P(D)$ of degree $N\geq1$, with leading coefficient $a_N$, we may choose the single staircase contour below every pole. Take $\gamma>\max\{\operatorname{Re}\lambda:P(\lambda)=0\}$ and integrate on $\operatorname{Im}\zeta=-\gamma$. The corresponding formula is the [Bromwich contour](../../../../../bromwich-contour.md) version of the construction above, after putting $\lambda=i\zeta$. Its poles all lie above the frequency contour. For $x<0$, close that contour downwards; the [exponential function](../../../../../exponential-function.md) $e^{ix\zeta}$ decays and there are no enclosed poles. For $x>0$, close upwards, where the [exponential function](../../../../../exponential-function.md) again decays, and apply the [residue theorem](../../../../../residue-theorem.md). The bound $1/P(i\zeta)=O(|\zeta|^{-N})$ justifies the large arcs, including $N=1$ by the [Jordan lemma](../../../../../jordan-s-lemma.md) away from their endpoints. Thus away from $x=0$ the [retarded fundamental solution](../../../../../retarded-fundamental-solution.md) is $H(x)u(x)$, where

$$
\boxed{u(x)=\sum_{P(\lambda)=0}\operatorname*{Res}_{z=\lambda}\frac{e^{zx}}{P(z)}.}
$$

The sum is over distinct [roots of a polynomial](../../../../../root-of-a-polynomial.md), with the residue including the whole multiplicity. For simple [characteristic roots of a constant-coefficient differential equation](../../../../../characteristic-root-of-a-constant-coefficient-differential-equation.md), it reduces to $u(x)=\sum_\lambda e^{\lambda x}/P'(\lambda)$. Repeated roots give [exponential polynomial solutions of a constant-coefficient differential equation](../../../../../exponential-polynomial-solution-of-a-constant-coefficient-differential-equation.md) through differentiation of $e^{zx}$.

To establish the equality also at the origin, rather than leave a possible point-supported term undecided, verify the [distributional jump formula for a Heaviside product](../../../../../distributional-jump-formula-for-a-heaviside-product.md). The residue expression is an [entire function](../../../../../entire-function.md) of $x$, and

$$
P(D)u(x)=\sum_\lambda\operatorname*{Res}_{z=\lambda}e^{zx}=0.
$$

Its initial derivatives are

$$
u^{(j)}(0)=\sum_\lambda\operatorname*{Res}_{z=\lambda}\frac{z^j}{P(z)}
=0\quad(0\leq j\leq N-2),\qquad u^{(N-1)}(0)=a_N^{-1}.
$$

These identities follow by integrating over a large circle: for $j\leq N-2$ the integrand is $O(|z|^{-2})$, whereas for $j=N-1$ its coefficient of $z^{-1}$ is $a_N^{-1}$. The [distributional jump formula for a Heaviside product](../../../../../distributional-jump-formula-for-a-heaviside-product.md) therefore gives $L(Hu)=\delta_0$. Moreover, since $e^{-\gamma x}Hu$ is a [tempered distribution](../../../../../tempered-distribution.md), its [Fourier transform](../../../../../fourier-transform.md) satisfies

$$
P(i\xi+\gamma)\widehat{e^{-\gamma x}Hu}(\xi)=1.
$$

There are no real zeros of this polynomial, so its reciprocal is the transform. This is exactly the shifted-contour construction, proving equality there as a [distribution](../../../../../distribution-mathematical-analysis.md) as well. Hence

$$
\boxed{E=Hu,\qquad Lu=0,\qquad LE=\delta_0,\qquad\operatorname{supp}E\subset[0,\infty).}
$$

The sign of $a_N$ matters: for the operator in the preceding solution, $a_N=-1$ and the last initial derivative is $-1$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

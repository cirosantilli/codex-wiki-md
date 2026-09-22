<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $M=\sup_{y>0}\int_{\mathbb R}|f(x+iy)|\,dx$. The goal is to obtain an integrable [non-tangential maximal function](../../../../../non-tangential-maximal-function.md) without assuming in advance that $f$ has an integrable boundary density. We use a square root to place the boundary data in $L^2$, where the [Hardy-Littlewood maximal function](../../../../../hardy-littlewood-maximal-function.md) is strongly bounded.

First recall this strong bound directly from Q2. For a nonnegative $h\in L^2(\mathbb R)$ and $\lambda>0$, split $h=h\mathbf1_{\{h>\lambda/2\}}+h\mathbf1_{\{h\leq\lambda/2\}}$. The second summand has centered maximal function at most $\lambda/2$; the first is in $L^1$. Q2's weak estimate, in dimension one, therefore gives

$$
|\{mh>\lambda\}|\leq\frac6\lambda\int_{\{h>\lambda/2\}}h.
$$

The [layer cake representation](../../../../../layer-cake-representation.md) and [Tonelli theorem](../../../../../tonelli-theorem.md) then imply

$$
\|mh\|_2^2=2\int_0^\infty\lambda|\{mh>\lambda\}|\,d\lambda
\leq12\int h(s)\int_0^{2h(s)}d\lambda\,ds=24\|h\|_2^2.
$$

This is the needed [Strong Lp bound for the Hardy-Littlewood maximal function](../../../../../strong-lp-bound-for-the-hardy-littlewood-maximal-function.md), with an explicit adequate constant.

For $\varepsilon>0$, let $f_\varepsilon(z)=f(z+i\varepsilon)$ and $h_\varepsilon(x)=|f(x+i\varepsilon)|^{1/2}$. Q1's elementary harmonic pointwise estimate makes $f_\varepsilon$ bounded on the closed upper half-plane. Its boundary value is continuous, and $\|h_\varepsilon\|_2^2\leq M$. The function $|f_\varepsilon|^{1/2}$ is [subharmonic](../../../../../subharmonic-function.md): away from zeros, for any $q>0$,

$$
\Delta |f_\varepsilon|^q=q^2|f_\varepsilon|^{q-2}|f_\varepsilon'|^2\geq0,
$$

and regularization, or the submean inequality at zeros, extends this to the whole domain. Bounded subharmonic comparison with the [Poisson integral](../../../../../poisson-integral.md) gives

$$
|f_\varepsilon(x'+iy)|^{1/2}\leq(P_y*h_\varepsilon)(x').
$$

Here $h_\varepsilon$ need not be in $L^1$. The [Poisson integral](../../../../../poisson-integral.md) is nevertheless defined, since $h_\varepsilon\in L^2\cap L^\infty$ and $P_y\in L^1\cap L^2$, and it tends to its continuous boundary values. To justify comparison on this unbounded domain, the difference between the two sides is bounded above, subharmonic, and zero on the real boundary. On an upper half-disk of radius $R$, use the positive harmonic barrier

$$
b_R(z)=\frac{2R\operatorname{Im}z}{|R-z|^2}+\frac{2R\operatorname{Im}z}{|R+z|^2}.
$$

On its semicircular arc, $b_R(Re^{i\theta})=2/\sin\theta\geq2$, while $b_R(z)\to0$ for every fixed interior $z$ as $R\to\infty$. The [maximum principle for subharmonic functions](../../../../../maximum-principle-for-subharmonic-functions.md), with a fixed bound for the difference, proves the comparison. The barrier's positive blow-up at the arc endpoints causes no difficulty.

For $|x-x'|\leq y$, the elementary inequality $y^2+|x-s|^2\leq3(y^2+|x'-s|^2)$ gives

$$
P_y(x'-s)\leq3P_y(x-s).
$$

Q2's [radial decreasing kernel domination by the maximal function](../../../../../radial-decreasing-kernel-domination-by-the-maximal-function.md) extends to nonnegative $L^2$ inputs by applying it to increasing bounded compactly supported truncations. Hence, taking the supremum over the cone,

$$
\bigl(f_\varepsilon^*(x)\bigr)^{1/2}\leq3m(h_\varepsilon)(x),\qquad
\int f_\varepsilon^*\leq9\|m(h_\varepsilon)\|_2^2\leq216M.
$$

For any fixed cone point, $f_\varepsilon(z)\to f(z)$ as $\varepsilon\downarrow0$. Therefore $f^*(x)\leq\liminf_{\varepsilon\downarrow0}f_\varepsilon^*(x)$; use a sequence of positive shifts and the [Fatou lemma](../../../../../fatou-s-lemma.md) to conclude

$$
\boxed{\int_{\mathbb R}f^*(x)\,dx\leq216\sup_{y>0}\int_{\mathbb R}|f(x+iy)|\,dx<\infty.}
$$

The precise numerical constant is unimportant. Suprema over countable dense sets of cone points give the same values, so the maximal functions used here are measurable.

This yields boundary [absolute continuity of measures](../../../../../absolute-continuity-of-measures.md) rather than assuming it. The [holomorphic function](../../../../../holomorphic-function.md) $f$ is a complex-valued [harmonic function](../../../../../harmonic-function.md), so Q1 represents it as $f(x+iy)=P_y*\mu(x)$ for a finite complex measure $\mu$, with $f(\cdot+iy)\,dx\to\mu$ weak-star. Since $|f(x+iy)|\leq f^*(x)$, every compactly supported continuous $\psi$ satisfies

$$
\left|\int\psi\,d\mu\right|\leq\int|\psi(x)|f^*(x)\,dx.
$$

The dual characterization of the [total variation measure](../../../../../variation-measure.md) implies $|\mu|\leq f^*\,dx$, so the [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) gives $\mu=F\,dx$ with $F\in L^1$. The [approximate identity](../../../../../approximate-identity.md) now gives $f(\cdot+iy)\to F$ in the [L1 norm](../../../../../l1-norm.md) and [almost everywhere](../../../../../almost-everywhere.md). Thus the analytic [Hardy space](../../../../../hardy-space.md) has an integrable boundary function, unlike the unrestricted harmonic $h^1$ space.

In the real-line form of the [F. and M. Riesz theorem](../../../../../f-and-m-riesz-theorem.md), start with a finite complex measure whose [Fourier transform of a finite measure](../../../../../fourier-transform-of-a-finite-measure.md) vanishes for $\xi<0$. Its [Poisson integral](../../../../../poisson-integral.md) is holomorphic: the transformed operators $\partial_y$ and $i\partial_x$ act by $-|\xi|$ and $-\xi$, which agree on that spectrum. These identities can first be read as distributional identities and then classically, since the [Poisson integral](../../../../../poisson-integral.md) is smooth. Its harmonic $h^1$ [norm](../../../../../norm.md) is finite by Q1, so the preceding argument makes the measure absolutely continuous. **A one-sided Fourier spectrum forces a finite boundary measure to have a Lebesgue density.**

For the customary circle form, normalize arc length by $dm=d\theta/(2\pi)$. If $\widehat\mu(n)=\int e^{-in\theta}\,d\mu(\theta)=0$ for $n<0$, then

$$
F(w)=\sum_{n\geq0}\widehat\mu(n)w^n,\qquad |w|<1,
$$

is analytic and $F(re^{i\theta})$ is the [Poisson integral on the unit disk](../../../../../poisson-integral-on-the-unit-disk.md) of $\mu$. Positivity and unit mass of the [Poisson kernel on the circle](../../../../../poisson-kernel-on-the-circle.md) imply $\sup_r\int|F(re^{i\theta})|\,dm\leq\|\mu\|_{\mathrm{TV}}$. The same square-root argument on the disk gives an integrable radial maximum, as follows. For $0<\rho<1$, put $h_\rho(\theta)=|F(\rho e^{i\theta})|^{1/2}$. The [maximum principle for subharmonic functions](../../../../../maximum-principle-for-subharmonic-functions.md) on the disk gives

$$
|F(\rho r e^{i\theta})|^{1/2}\leq(P_r*h_\rho)(\theta).
$$

The supremum of these [Poisson integrals](../../../../../poisson-integral.md) is bounded by a constant times the circular [Hardy-Littlewood maximal function](../../../../../hardy-littlewood-maximal-function.md). Indeed, for $r\geq1/2$ the circular kernel is bounded by a constant times $(1-r)/((1-r)^2+\theta^2)$ for $|\theta|\leq\pi$; splitting into arcs of radii $2^j(1-r)$ gives a summable geometric series of arc averages. For $r<1/2$ the kernel is uniformly bounded, and the whole-circle average suffices. The covering proof and the truncation argument already used on the line give the strong $L^2$ maximal bound for arcs on the circle as well. Thus

$$
\int\sup_{0<r<1}|F(\rho r e^{i\theta})|\,dm
\leq C\|h_\rho\|_2^2\leq C\|\mu\|_{\mathrm{TV}}.
$$

Let $\rho\uparrow1$ and apply [Fatou lemma](../../../../../fatou-s-lemma.md) to obtain an integrable radial maximum $R(\theta)=\sup_{0<r<1}|F(re^{i\theta})|$. The measures $F(re^{i\theta})\,dm$ tend weak-star to $\mu$ and are dominated in magnitude by $R\,dm$. The same continuous-test-function argument gives $|\mu|\leq R\,dm$. This proves **the F. and M. Riesz theorem: a finite complex measure on the circle with all negative Fourier coefficients zero is absolutely continuous with respect to arc length**. Reversing the Fourier convention interchanges positive and negative indices.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

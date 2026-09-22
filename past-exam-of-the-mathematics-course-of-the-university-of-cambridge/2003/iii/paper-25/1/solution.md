<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We give a spectral proof of [square-difference recurrence for finite colourings](../../../../../square-difference-recurrence-for-finite-colourings.md), proving the auxiliary results it uses. Extend the colouring arbitrarily to nonpositive integers, and let $f_j$ be the indicator of colour $j$. By successively taking subsequences of the interval lengths, followed by a diagonal subsequence, we may arrange that all the limits

$$
\delta_j=\lim_{L\to\infty}\frac1L\sum_{x=1}^Lf_j(x),\qquad
c(h)=\lim_{L\to\infty}\frac1L\sum_{x=1}^L\sum_{j=1}^r f_j(x)f_j(x+h)
$$

exist, for every integer $h$. This uses only sequential compactness of bounded real sequences: list the countably many quantities, choose a convergent subsequence for each in turn, and take the diagonal. All limits below are along this common subsequence. We have $c(0)=1$, $c(-h)=c(h)$, $c(h)\ge0$ and $\sum_j\delta_j=1$. Translating a fixed interval endpoint changes a normalized average by $O(|h|/L)$.

The sequence is a [positive-definite function](../../../../../positive-definite-function.md) on $\mathbb Z$. Indeed, for finitely many complex numbers $z_u$,

$$
\sum_{u,v}z_u\overline{z_v}c(u-v)
=\lim_{L\to\infty}\frac1L\sum_x\sum_j
\left|\sum_uz_uf_j(x+u)\right|^2\ge0.
$$

We next prove the required [Bochner–Herglotz theorem](../../../../../bochner-herglotz-theorem.md) for this sequence. The trigonometric polynomial

$$
F_H(t)=\sum_{|h|<H}(1-|h|/H)c(h)e(-ht)
=\frac1H\sum_{u,v=0}^{H-1}c(u-v)e(-ut)e(vt)
$$

is nonnegative by positive definiteness, and its integral on the circle is $c(0)=1$. Thus $F_H(t)\,dt$ is a probability measure. Such measures on a compact interval have a weakly convergent subsequence. For completeness, take a diagonal subsequence on all rational points of their nondecreasing distribution functions. The right-continuous extension of the limiting rational values is a distribution function and defines a probability measure by its interval increments. At its continuity points the original distribution functions converge, by sandwiching between rational endpoints. Approximating continuous functions by step functions with such endpoints proves convergence of their integrals. Identify the interval endpoints to obtain a measure on the circle. This proves the [compactness of probability measures on a compact metric space](../../../../../compactness-of-probability-measures-on-a-compact-metric-space.md) in the case needed here.

For a fixed $h$, the Fourier coefficient of $F_H\,dt$ is $(1-|h|/H)c(h)$ once $H>|h|$. Taking the weak limit therefore supplies a positive probability measure $\mu$ such that

$$
c(h)=\int_{\mathbb R/\mathbb Z}e(ht)\,d\mu(t).
$$

No spectral representation has been assumed without proof.

Its atom at zero has positive mass. For each $H$,

$$
\int\left|\frac1H\sum_{u=0}^{H-1}e(ut)\right|^2d\mu(t)
=\lim_{L\to\infty}\frac1L\sum_x\sum_j
\left(\frac1H\sum_{u=0}^{H-1}f_j(x+u)\right)^2
\ge\sum_j\delta_j^2.
$$

The last inequality is Cauchy-Schwarz on each colour's interval average. The integrand is at most one and tends to zero for every nonzero point of the circle, by the geometric-series formula, while it is one at zero. Bounded convergence gives

$$
\mu(\{0\})\ge\sum_j\delta_j^2\ge1/r.
$$

We also prove that quadratic phases with an irrational coefficient average to zero. For $z_0,\ldots,z_{L-1}$ bounded by one, extended by zero, Cauchy-Schwarz applied to $\sum_x\sum_{u=0}^{H-1}z_{x+u}=H\sum_xz_x$ yields

$$
H^2\left|\sum_xz_x\right|^2
\le(L+H-1)\left(HL+2\sum_{h=1}^{H-1}(H-h)
\left|\sum_xz_{x+h}\overline{z_x}\right|\right).
$$

This identity follows by expanding the square of the inner shifted sum and grouping pairs by their difference; it is the needed finite [Van der Corput inequality for finite scalar sequences](../../../../../van-der-corput-inequality-for-finite-scalar-sequences.md). If $z_x=e(\theta x^2)$ and $\theta$ is irrational, each fixed nonzero lag correlation is a geometric sum with frequency $2\theta h$, hence is bounded independently of $L$. The geometric bound follows from $(1-z^L)/(1-z)$ with $z=e(2\theta h)\ne1$. Dividing by $H^2L^2$ and letting $L$ tend to infinity gives $\limsup|L^{-1}\sum z_x|^2\le1/H$. Letting $H$ tend to infinity proves the asserted cancellation. Rational coefficients instead give periodic sequences and therefore have convergent averages.

Choose a finite set $T$ of rational points of the circle, including zero, such that the total mass of the remaining rational atoms is below $1/(2r)$. This is possible because the rational points are countable and $\mu$ is finite. Let $q$ be a common multiple of their denominators. For $t\in T$, $e(tq^2m^2)=1$ for every integer $m$. For irrational $t$ the preceding cancellation applies to $q^2t$; at every other rational point the average exists by periodicity and has modulus at most one. Bounded convergence consequently gives

$$
\lim_{H\to\infty}\frac1H\sum_{m=1}^Hc((qm)^2)
=\int\lim_{H\to\infty}\frac1H\sum_{m=1}^He(tq^2m^2)\,d\mu(t)
\ge\mu(T)-\frac1{2r}\ge\frac1{2r}>0.
$$

Here the inequality takes real parts; $c$ itself is real. Thus some $b=qm>0$ has $c(b^2)>0$. By its definition as a limit of nonnegative averages, at least one actual positive $a$ has $\sum_jf_j(a)f_j(a+b^2)>0$. The same colour occurs at both points, proving

$$
\boxed{\phi(a)=\phi(a+b^2)\quad\text{for some }a,b>0.}
$$

The arbitrary extension to nonpositive integers played no role in this final pair.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

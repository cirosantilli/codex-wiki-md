<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The interior [elliptic regularity](../../../../../../elliptic-regularity.md) assertion for the [Laplace equation](../../../../../../laplace-equation.md) is that a [harmonic function](../../../../../../harmonic-function.md) is [smooth](../../../../../../smooth-function.md), in fact [real analytic](../../../../../../real-analytic-function.md), throughout $U$. No boundary regularity of its unspecified boundary values is implied.

First let $u\in C^2(U)$ and $\Delta u=0$. On a ball compactly contained in $U$, differentiating its spherical average and applying the [divergence theorem](../../../../../../divergence-theorem.md) expresses that derivative as a constant factor times $\int_{B_r}\Delta u$, which is zero. The spherical average tends to $u$ at the center as $r\to0$. This proves the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md).

Choose a radially symmetric [smooth](../../../../../../smooth-function.md) [mollifier](../../../../../../mollifier.md) $\eta_r$, supported in $B_r$, with integral one. By integrating the spherical [mean value property](../../../../../../mean-value-property-for-harmonic-functions.md),

$$
u(x)=\int\eta_r(x-y)u(y)\,dy
$$

whenever $B_r(x)\Subset U$. For fixed $r$ the right side is a [smooth](../../../../../../smooth-function.md) [convolution](../../../../../../convolution.md), since all [derivatives](../../../../../../derivative.md) can be placed on $\eta_r$. Thus $u$ is [smooth](../../../../../../smooth-function.md). The same argument proves the [Weyl lemma](../../../../../../weyl-lemma.md) for a distributionally [harmonic](../../../../../../harmonic-function.md) $u\in L^1_{\mathrm{loc}}$: first mollify $u$, apply the fixed-radius identity, and let the mollification radius tend to zero in distributions to obtain the same smooth representative.

To prove [real analytic](../../../../../../real-analytic-function.md) regularity, differentiating the fixed-radius [convolution](../../../../../../convolution.md) gives the [interior derivative estimate for a harmonic function](../../../../../../interior-derivative-estimate-for-a-harmonic-function.md)

$$
|\partial_j v(x)|\leq\frac{C_\ell}{r}\sup_{B_r(x)}|v|
$$

for any [harmonic](../../../../../../harmonic-function.md) $v$. All [derivatives](../../../../../../derivative.md) of $u$ are [harmonic](../../../../../../harmonic-function.md). On nested balls between $B_R(a)$ and $B_{R/2}(a)$, apply this estimate $k$ times, decreasing the radius by $R/(2k)$ each time. For $|\alpha|=k$,

$$
\sup_{B_{R/2}(a)}|D^\alpha u|\leq\left(\frac{Ck}{R}\right)^k\sup_{B_R(a)}|u|
\leq\left(\frac{Ce}{R}\right)^k k!\sup_{B_R(a)}|u|.
$$

The inequality $k^k\leq e^k k!$ follows by integrating $\log s$ below the sum defining $\log(k!)$. Apply the one-dimensional [Taylor theorem](../../../../../../taylor-theorem.md) along each segment, expanding directional [derivatives](../../../../../../derivative.md) by the multinomial formula. The remainder is bounded by $M(A\sum_j|h_j|)^k$, so it tends to zero for sufficiently small $h$. This gives a locally convergent multivariate [Taylor series](../../../../../../taylor-series.md). **A [harmonic function](../../../../../../harmonic-function.md) is [real analytic](../../../../../../real-analytic-function.md) in the interior.**

The usual inhomogeneous [elliptic regularity](../../../../../../elliptic-regularity.md) statement also follows: if $\Delta u=f$ and $f$ is [smooth](../../../../../../smooth-function.md), take a cutoff $\chi$ equal to one near a given point and set $w=\Phi*(\chi f)$, where $\Phi$ is a [fundamental solution of the Laplace equation](../../../../../../fundamental-solution-of-the-laplace-equation.md) with $\Delta\Phi=\delta$. Moving every [derivative](../../../../../../derivative.md) to the compactly supported [smooth](../../../../../../smooth-function.md) function $\chi f$ shows $w$ is [smooth](../../../../../../smooth-function.md). Locally $u-w$ is [harmonic](../../../../../../harmonic-function.md), so $u$ is [smooth](../../../../../../smooth-function.md) there too.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

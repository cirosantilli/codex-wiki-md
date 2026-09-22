<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose real normalized [eigenfunctions](../../../../../../eigenfunction.md), including the two [zero-energy filament modes](../../../../../../zero-energy-filament-mode.md). The expansion is

$$
h=a_{\rm tr}W_{\rm tr}+a_{\rm tilt}W_{\rm tilt}+\sum_{n\geq1}a_nW_n.
$$

[Integration by parts](../../../../../../integration-by-parts.md) with the natural endpoints gives $\int W_m''W_n''dx=k_n^4\delta_{mn}$. Hence

$$
\mathcal E=\frac A2\sum_{n\geq1}k_n^4a_n^2.
$$

For each positive mode, the [equipartition theorem](../../../../../../equipartition-theorem.md) gives

$$
\boxed{\langle a_n^2\rangle=\frac{k_BT}{Ak_n^4}.}
$$

Distinct modal amplitudes are independent centered [Gaussian random variables](../../../../../../gaussian-random-variable.md) in the canonical bending ensemble.

The rigid translation and tilt amplitudes have no energy cost. Their integrals in the [canonical ensemble](../../../../../../canonical-ensemble.md) are unbounded, so **a completely free filament has no normalizable equilibrium height distribution and no finite height [variance](../../../../../../variance-split.md) determined by this energy alone**. This is a physical qualification of the requested [variance](../../../../../../variance-split.md), not a reason to omit the bending fluctuations.

Fixing translation and tilt, for example by imposing $\int h\,dx=\int(x-L/2)h\,dx=0$, leaves the [rigid-motion-projected thermal covariance of a free filament](../../../../../../rigid-motion-projected-thermal-covariance-of-a-free-filament.md):

$$
\boxed{C(x,y)=\frac{k_BT}{A}\sum_{n\geq1}\frac{W_n(x)W_n(y)}{k_n^4},\qquad
\operatorname{Var}h(x)=\frac{k_BT}{A}\sum_{n\geq1}\frac{W_n(x)^2}{k_n^4}.}
$$

For unnormalized modes, divide each summand by $\int W_n^2dx$. Any prescribed independent [variance](../../../../../../variance-split.md) of the two rigid amplitudes must be added separately; [equipartition theorem](../../../../../../equipartition-theorem.md) does not assign it.

The [free-filament variance with fixed translation and tilt](../../../../../../free-filament-variance-with-fixed-translation-and-tilt.md) also has a closed form. Integrate a [white noise](../../../../../../white-noise.md) curvature field twice, and subtract its affine least-squares projection. With $u=x/L$, $t=s/L$, the dimensionless kernel is

$$
\mathcal K(u,t)=(u-t)_+-\frac{(1-t)^2}{2}
-(1-3t^2+2t^3)(u-\tfrac12).
$$

It has zero mean and first spatial moment, while its second $u$ derivative is the delta source. Since the [covariance](../../../../../../covariance.md) is $(k_BT/A)\delta(s-s')$, integrate its squared kernel to obtain

$$
\boxed{\operatorname{Var}h(x)=\frac{k_BTL^3}{A}P(u),\qquad
P(u)=\frac1{105}-\frac{11u}{105}+\frac{13u^2}{35}-\frac{u^3}{3}
-\frac{u^4}{3}+\frac{3u^5}{5}-\frac{u^6}{5}.}
$$

This conditional profile is symmetric about the midpoint: $P(1-u)=P(u)$, with endpoint value $1/105$ and midpoint value $1/320$. It refers to removing the free rigid motion, not to clamping either end.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

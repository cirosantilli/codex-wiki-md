<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use $\hbar=c=k_B=1$ and normalize the time-translation [Killing vector field](../../../../../killing-vector-field.md) at infinity. The simple outer zero and positivity on its exterior imply $b=V'(r_0)>0$. Near the horizon, write $x=r-r_0$; then $V=bx+O(x^2)$. The [Wick rotation](../../../../../wick-rotation.md) $t=-it_E$ gives the radial Euclidean metric

$$
ds_E^2=V\,dt_E^2+\frac{dr^2}{V}+r^2d\Omega^2.
$$

Define $\rho=2\sqrt{x/b}$, so $x=b\rho^2/4$. Its leading near-horizon form is

$$
ds_E^2=d\rho^2+\rho^2\left(\frac b2dt_E\right)^2+r_0^2d\Omega^2+O(\rho^2)d\rho^2+O(\rho^4)dt_E^2+O(\rho^2)d\Omega^2.
$$

Thus $bt_E/2$ is a polar angle. Smoothness at the origin requires period $2\pi$, rather than a cone or a multiple cover with a branched origin. The [Euclidean black-hole regularity condition](../../../../../euclidean-black-hole-regularity-condition.md) is

$$
\beta=\frac{4\pi}{b}.
$$

A thermal quantum state has imaginary-time period $\beta=1/T$. Since $V\to1$, this time coordinate is normalized to the clocks at infinity, and the [Hawking temperature](../../../../../hawking-temperature.md) is

$$
\boxed{T=\frac{V'(r_0)}{4\pi}.}
$$

A static clock at radius $r>r_0$ measures the redshifted local temperature $T/\sqrt{V(r)}$; that local quantity is not the temperature requested with the asymptotic normalization.

The static coordinates are singular on the horizon, so calculate its [surface gravity](../../../../../surface-gravity.md) in a regular ingoing chart. With $v=t+\int dr/V$, the metric and the same normalized [Killing vector field](../../../../../killing-vector-field.md) are

$$
ds^2=-V\,dv^2+2\,dv\,dr+r^2d\Omega^2,\qquad k=\partial_v.
$$

The inverse radial block has $g^{vr}=1$, $g^{rr}=V$, $g^{vv}=0$. Direct calculation gives

$$
\Gamma^v{}_{vv}=\frac{V'}2,\qquad\Gamma^r{}_{vv}=\frac{VV'}2.
$$

Since $k$ has constant coordinate components, its acceleration is

$$
k^a\nabla_a k^b=\frac{V'}2(\partial_v)^b+\frac{VV'}2(\partial_r)^b.
$$

On the future horizon, $V=0$ and $k$ is null, so the defining equation gives $\kappa=b/2$. In the outgoing chart regular on the past branch, the radial cross-term is $-2\,du\,dr$ and the same calculation gives $\kappa=-b/2$ for $k=\partial_u$. Hence the branch-independent physical statement is

$$
\boxed{|\kappa|=\frac{V'(r_0)}2=2\pi T.}
$$

This proves the [Euclidean temperature and signed horizon surface gravity](../../../../../euclidean-temperature-and-signed-horizon-surface-gravity.md) relation directly. Rescaling the [Killing vector field](../../../../../killing-vector-field.md) would rescale its [surface gravity](../../../../../surface-gravity.md); the condition at infinity fixes that otherwise arbitrary normalization.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="24i/solution">Solution</h1>

↑ **Parent:** [24I](../24i.md)

The [Gauss map](../../../../../gauss-map.md) of an oriented surface is its smooth unit normal $N:S\to S^2$. With the convention that the [shape operator](../../../../../shape-operator.md) is $A_p=-dN_p$, the [second fundamental form](../../../../../second-fundamental-form-split.md) is $\mathrm{II}_p(v,w)=\langle A_pv,w\rangle$ and the [normal curvature](../../../../../normal-curvature.md) in a nonzero direction $w$ is $k_n(w)=\mathrm{II}(w,w)/\langle w,w\rangle$. The two [principal curvatures](../../../../../principal-curvature.md) are the real eigenvalues $k_1,k_2$ of this self-adjoint operator; the [mean curvature](../../../../../mean-curvature.md) is $H=(k_1+k_2)/2$.

For directions successively spaced around the tangent plane, write their angles to a principal direction as $\theta_j=\theta_0+(j-1)\pi/m$. The [Euler formula for normal curvature](../../../../../euler-formula-for-normal-curvature.md) gives

$$
\widetilde k_j=k_1\cos^2\theta_j+k_2\sin^2\theta_j=H+\frac{k_1-k_2}{2}\cos(2\theta_j).
$$

The [geometric series](../../../../../geometric-series.md) $\sum_{j=0}^{m-1}e^{2\pi ij/m}=0$ for $m\geq2$ makes the cosine sum zero. Therefore

$$
\boxed{\sum_{j=1}^m\widetilde k_j=mH.}
$$

Here equal angular spacing is understood in the usual directed sense. If the printed consecutive angles were only unsigned, without requiring the same rotational sense, the assertion would be false: for $m=3$ the directions $0,\pi/3,0$ satisfy those unsigned angle conditions but do not generally give $3H$.

A [minimal surface](../../../../../minimal-surface.md) has $H=0$, so at each point $k_2=-k_1$. In an orthonormal principal basis, $A=\operatorname{diag}(k_1,-k_1)$ and $A^2=k_1^2I$. Hence

$$
\langle dN_p(w_1),dN_p(w_2)\rangle=\langle A_pw_1,A_pw_2\rangle=k_1^2\langle w_1,w_2\rangle,
$$

which proves the identity with $\boxed{\mu(p)=k_1^2=-K(p)\geq0}$, where $K$ is the [Gaussian curvature](../../../../../gaussian-curvature.md).

The converse is false. The identity only forces $k_1^2=k_2^2$, which allows either $k_2=-k_1$ or $k_2=k_1$. A sphere of radius $R$ has $dN=I/R$ for its outward normal, so it satisfies the identity with $\mu=R^{-2}$, yet $H=-1/R\ne0$ under the chosen convention. Thus a conformal Gauss map can also arise from an umbilic nonminimal surface.

## ↑ Ancestors (10)

1. [24I](../24i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

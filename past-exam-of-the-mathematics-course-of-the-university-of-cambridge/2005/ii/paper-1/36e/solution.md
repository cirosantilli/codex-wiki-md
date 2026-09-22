<h1 id="36e/solution">Solution</h1>

↑ **Parent:** [36E](../36e.md)

For steady unidirectional [pressure-driven channel flow](../../../../../pressure-driven-channel-flow.md), write $G=-dp/dz>0$. The axial [momentum](../../../../../momentum.md) equation and [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) are

$$
\boxed{\nabla_\perp^2w=-G/\mu\quad\text{in }D,\qquad w=0\quad\text{on }\partial D.}
$$

Near an ideal wedge, the constant forcing has an $r^2$ particular solution by scaling. Substitution gives $f''+4f=-1$, with $f(\pm\alpha)=0$. For $\cos2\alpha\ne0$, the symmetric particular solution is

$$
\boxed{f(\theta)=\tfrac14\left(\frac{\cos2\theta}{\cos2\alpha}-1\right).}
$$

This [corner expansion of pressure-driven sector flow](../../../../../corner-expansion-of-pressure-driven-sector-flow.md) is a particular solution, not necessarily the dominant corner term; a homogeneous corner mode can be larger, as the requested cases below show.

Separation of the symmetric harmonic correction with zero values on the straight walls gives modes $r^{\lambda_n}\cos(\lambda_n\theta)$, where

$$
\boxed{\lambda_n=\frac{(2n+1)\pi}{2\alpha},\qquad n=0,1,\ldots.}
$$

Regularity at the vertex excludes negative powers. [Orthogonality](../../../../../orthogonal-vectors.md) on $[-\alpha,\alpha]$ has norm $\alpha$. To cancel the particular solution on $r=a$, use its [cosine](../../../../../cosine.md) coefficients

$$
f_n=\frac1\alpha\int_{-\alpha}^{\alpha}f(\theta)\cos(\lambda_n\theta)d\theta=\frac{2(-1)^n}{\alpha\lambda_n(\lambda_n^2-4)}.
$$

The [integral](../../../../../integral.md) follows by product-to-sum and $\sin(\lambda_n\alpha)=(-1)^n$. Thus

$$
\boxed{w=\frac G\mu r^2f(\theta)+\sum_{n\ge0}A_nr^{\lambda_n}\cos(\lambda_n\theta),\qquad A_n=\frac{2(G/\mu)(-1)^na^{2-\lambda_n}}{\alpha\lambda_n(4-\lambda_n^2)}.}
$$

The arc data are satisfied by the [cosine](../../../../../cosine.md) expansion, and the [Poisson equation](../../../../../poisson-equation.md) by construction. At the omitted thresholds $2\alpha=\pi/2,3\pi/2$, a mode has $\lambda_n=2$, so the pure $r^2f$ ansatz is resonant. The corresponding finite-limit term in the full sector solution is $(G/\mu)(-1)^nr^2\log(a/r)\cos2\theta/(4\alpha)$; the other modes remain regular. This explains rather than hides the division by $\cos2\alpha$.

## ↑ Ancestors (10)

1. [36E](../36e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

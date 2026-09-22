<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take the first centre at the origin. If some listed centres coincide, first combine their poles; let $M$ be the total residue at the origin, so $M=M_1$ when the centres are distinct. The contributions from centres away from the origin are real analytic there. Their constant term is

$$
\boxed{h=1+\sum_{\mathbf x_j\ne0}\frac{M_j}{|\mathbf x_j|},\qquad H=\frac Mr+h+rF(r,\theta,\phi),}
$$

where $F$ is analytic in $r$ and in local angular charts. This follows by substituting $\mathbf x=r\mathbf n(\theta,\phi)$ in the ordinary [Taylor expansions](../../../../../../../taylor-expansion.md) of the regular contributions. The constant $h$ is independent of angle, which makes the hinted coordinate differential integrable.

Put $A=M+hr$, $Q=rH=A+r^2F$, and define

$$
v=t+h^2r+2hM\log r-\frac{M^2}{r},\qquad dv=dt+\left(h+\frac Mr\right)^2dr
$$

initially for $r>0$. Substitution into the metric gives

$$
ds^2=-\frac{r^2}{Q^2}dv^2+2\frac{A^2}{Q^2}dv\,dr+\frac{Q^4-A^4}{r^2Q^2}dr^2+Q^2d\Omega_2^2.
$$

The apparently singular radial coefficient is actually

$$
\frac{Q^4-A^4}{r^2Q^2}=F\frac{(Q+A)(Q^2+A^2)}{Q^2},
$$

since $Q-A=r^2F$. All coefficients therefore extend analytically to negative and positive $r$ near zero, with $Q(0)=M>0$. At the horizon $g_{vv}=0$, $g_{vr}=1$, $g_{rr}=4MF(0,\theta,\phi)$ and the angular metric is $M^2d\Omega_2^2$. The $v,r$ determinant is $-1$ both before and at the extension, so the metric remains nondegenerate and Lorentzian. Angular coordinate singularities are handled by ordinary sphere charts. This explicitly constructs the [analytic extension of a Majumdar–Papapetrou horizon](../../../../../../../analytic-extension-of-a-majumdar-papapetrou-horizon.md).

Inverting the radial block gives $g^{rr}=r^2/Q^2$, which vanishes at $r=0$. Thus the hypersurface is null. Its normal agrees there with the metric dual of $\xi=\partial_v$: $\xi_a\,dx^a=dr$ on the horizon. The metric is independent of $v$, so $\xi$ is a [Killing vector field](../../../../../../../killing-vector-field.md) and the null hypersurface is a [Killing horizon](../../../../../../../killing-horizon.md).

The [surface gravity](../../../../../../../surface-gravity.md) obeys $\nabla_a(\xi^2)=-2\kappa\xi_a$ on a [Killing horizon](../../../../../../../killing-horizon.md). Here $\xi^2=-r^2/Q^2$ has a double zero and its entire differential vanishes at $r=0$, while $\xi_a$ is the nonzero normal. Consequently

$$
\boxed{\kappa=0.}
$$

The horizon is degenerate. Its cross-sectional area is $4\pi M^2$, independent of the centres away from the origin. The essential cancellation would fail with an arbitrary constant in place of the displayed regular part $h$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

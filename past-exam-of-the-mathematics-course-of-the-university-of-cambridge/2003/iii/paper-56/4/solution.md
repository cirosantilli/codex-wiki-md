<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $f(r)=1-2M/r+Q^2/r^2$. A positive-radius horizon requires a root of $r^2-2Mr+Q^2=0$, giving

$$
r_\pm=M\pm\sqrt{M^2-Q^2}.
$$

For the usual asymptotically flat [Reissner-Nordstrom spacetime](../../../../../reissner-nordstrom-spacetime.md), the black-hole conditions are

$$
\boxed{M>0,\qquad M\geq |Q|.}
$$

The strict inequality gives a nonextremal outer [event horizon](../../../../../event-horizon.md) at $r_+$; equality gives an [extremal black hole](../../../../../extremal-black-hole.md). If $M<|Q|$ with $M>0$, there is no horizon and the central [curvature singularity](../../../../../curvature-singularity.md) is naked. Nonpositive $M$ cannot supply a positive-radius black-hole horizon; $M=Q=0$ is [Minkowski spacetime](../../../../../minkowski-spacetime.md). For $Q=0$, the zero root $r_-=0$ is the singularity, not an additional regular horizon.

In the static coordinates the vector $k=\partial_t$ has constant components and every metric component is independent of $t$. Its [Lie derivative](../../../../../lie-derivative-of-a-differential-form.md) therefore satisfies

$$
(\mathcal L_k g)_{ab}=k^c\partial_cg_{ab}+g_{cb}\partial_ak^c+g_{ac}\partial_bk^c=0.
$$

For the torsion-free [Levi-Civita connection](../../../../../levi-civita-connection.md), $\mathcal L_k g=2\nabla_{(a}k_{b)}$, proving the [Killing equation](../../../../../killing-equation.md) directly. This also normalizes the [Killing vector field](../../../../../killing-vector-field.md) to unit time translation at infinity.

At $r=r_+$, $k^2=-f=0$. Use the regular advanced chart $v=t+r_*$ with $dr_*/dr=f^{-1}$, in which

$$
ds^2=-f\,dv^2+2\,dv\,dr+r^2d\Omega_2^2,\qquad k=\partial_v.
$$

On the horizon, $k_a=(dr)_a$. Thus the [Killing vector field](../../../../../killing-vector-field.md) is both null and normal to the horizon, and its orbits generate that [Killing horizon](../../../../../killing-horizon.md). The normal lines of a [null hypersurface](../../../../../null-hypersurface.md) are [null geodesics](../../../../../null-geodesic.md), possibly with nonaffine parameter. To see this without assuming a separate geodesic property, the [Killing equation](../../../../../killing-equation.md) gives

$$
k^a\nabla_a k_b=-k^a\nabla_b k_a=-\frac12\nabla_b(k^2)=\frac12f'(r)(dr)_b.
$$

Restriction to the future horizon therefore gives

$$
k^a\nabla_a k_b=\frac12f'(r_+)k_b.
$$

The acceleration is proportional to the tangent, which is exactly the [geodesic equation](../../../../../geodesic-equation.md) with a nonaffine parameter. An affinely parametrized tangent can be obtained by rescaling $k$ along each generator; that rescaled vector need not itself extend to a spacetime [Killing vector field](../../../../../killing-vector-field.md). At a nonextremal [bifurcation surface](../../../../../bifurcation-surface.md), $k$ vanishes, so a nonzero generator tangent must be described in a regular affine parametrization there.

On the past branch, use the retarded chart with radial-time cross term $-2\,du\,dr$. Now $k_a=-(dr)_a$ at the horizon, so the same calculation yields the opposite signed nonaffinity. Since $r_+$ is constant and the spacetime is spherically symmetric, $f'(r_+)/2$ is constant over the future horizon. This gives the two signs in the horizon relation without assuming their value beforehand.

Factor $f=(r-r_+)(r-r_-)/r^2$. Its derivative at the outer horizon gives the [Reissner-Nordstrom horizon surface gravity](../../../../../reissner-nordstrom-horizon-surface-gravity.md)

$$
\boxed{\kappa=\frac12 f'(r_+)=\frac{r_+-r_-}{2r_+^2}
=\frac{\sqrt{M^2-Q^2}}{\left(M+\sqrt{M^2-Q^2}\right)^2}.}
$$

It is positive for $M>|Q|$, and at $Q=0$ reduces to the [Schwarzschild surface gravity](../../../../../schwarzschild-surface-gravity.md) $1/(4M)$. For $M=|Q|>0$, the root is double and $\kappa=0$. Thus **the horizon remains present when its surface gravity vanishes**: it is a [degenerate Killing horizon](../../../../../degenerate-killing-horizon.md), and $k$ itself has affine parametrization along its nonzero horizon generators. The strictly positive-constant description applies only to the nonextremal case; the zero value is the legitimate extremal limit.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

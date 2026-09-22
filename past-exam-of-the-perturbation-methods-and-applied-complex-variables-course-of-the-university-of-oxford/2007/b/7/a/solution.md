<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [integral](../../../../../integral-split.md) construction requires differentiation under the [integral](../../../../../integral-split.md) and vanishing boundary terms. With those assumptions, [integration by parts](../../../../../integration-by-parts.md) gives

$$
w''+zw=[g(\zeta)e^{z\zeta}]_{\partial\Gamma}
+\int_\Gamma(\zeta^2g-g')e^{z\zeta}\,d\zeta.
$$

The standard construction therefore sets $g'=\zeta^2g$, giving $g=C e^{\zeta^3/3}$. Convergent [contours](../../../../../complex-integration-contour.md) run between rays where $\Re\zeta^3<0$: convenient central rays have arguments $-\pi/3$, $\pi/3$ and $\pi$. Two choices are the oriented paths

$$
\Gamma_1:\infty e^{-i\pi/3}\longrightarrow0\longrightarrow\infty e^{i\pi/3},
\qquad
\Gamma_2:\infty e^{i\pi/3}\longrightarrow0\longrightarrow-\infty.
$$

The cubic exponential dominates the linear one at both ends. To verify independence directly, put $A=\int_0^\infty e^{-r^3/3}dr>0$ and $B=\int_0^\infty r e^{-r^3/3}dr>0$. At $z=0$ the value and [derivative](../../../../../derivative.md) of the [integral](../../../../../integral-split.md) along rays $\theta_1,\theta_2$ are $A(e^{i\theta_2}-e^{i\theta_1})$ and $B(e^{2i\theta_2}-e^{2i\theta_1})$. For the two [contours](../../../../../complex-integration-contour.md) above their derivative-to-value ratios are respectively $B/A$ and $(B/A)(e^{i\pi/3}-1)$, which differ. Hence their [Wronskian](../../../../../wronskian.md) is nonzero.

For the second equation multiply by $z$ before integrating by parts:

$$
z(w''+w)+w'
=[(1+\zeta^2)g e^{z\zeta}]_{\partial\Gamma}
-\int_\Gamma\bigl((1+\zeta^2)g'+\zeta g\bigr)e^{z\zeta}d\zeta.
$$

Setting the residual weight to zero gives $g=C(1+\zeta^2)^{-1/2}$. One [contour](../../../../../complex-integration-contour.md) is the segment from $-i$ to $i$, with the [square root](../../../../../square-root.md) positive at $\zeta=0$. Its [integral](../../../../../integral-split.md) is a nonzero multiple of $J_0(z)$: substituting $\zeta=it$ gives $i\int_{-1}^1e^{izt}(1-t^2)^{-1/2}dt$, an [entire function](../../../../../entire-function.md) nonzero at zero.

A second [contour](../../../../../complex-integration-contour.md) starts at $i$ and follows $\zeta=i-t$, $0\leq t<\infty$, choosing a continuous branch along the path. For $\Re z>0$ it converges at infinity; at the branch endpoint its integrable singularity is $t^{-1/2}$. In both cases the boundary term contains $\sqrt{1+\zeta^2}$ and vanishes at branch endpoints. The second [integral](../../../../../integral-split.md) has a nonzero [logarithmic divergence](../../../../../logarithmic-divergence.md) as $z\to0$ through positive real values, because its large-$t$ integrand is a nonzero multiple of $e^{-zt}/t$. It is therefore independent of the entire first solution; [analytic continuation](../../../../../analytic-continuation.md) supplies solutions elsewhere away from the equation's singular point.

Strictly, nonzero $w$ and an arbitrary [contour](../../../../../complex-integration-contour.md) alone do not prove the printed necessity for $g$. Necessity also needs [injectivity](../../../../../injective-function.md) of the chosen Laplace representation, while the vanishing-integrand argument above is the usual sufficient construction. For a concrete counterexample to unconditional necessity in the Bessel case, take a positively oriented circle $|\zeta|=R>1$, choose the branch $(1+\zeta^2)^{-1/2}\sim1/\zeta$ outside the cut $[-i,i]$, and add one to that weight. The added entire integrand integrates to zero. Expanding the original weight on this circle gives [integral](../../../../../integral-split.md) $2\pi i J_0(z)$, which is nonzero and solves the equation, although the modified weight is not a constant multiple of the printed one. The standard weights and [contours](../../../../../complex-integration-contour.md) above still give the requested independent solutions.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Interpret the printed [Euclidean norm](../../../../../euclidean-norm.md) literally on the full vector array $X^2$. It is a single global [norm](../../../../../norm.md), not the sum of pixelwise [gradient](../../../../../gradient.md) lengths in [discrete isotropic total variation](../../../../../discrete-isotropic-total-variation.md). Set $A=\nabla$ and let $A^*$ be its exact [adjoint operator](../../../../../adjoint-operator.md) for the chosen difference and boundary conventions. The closed dual ball and its [image signal](../../../../../image-signal.md) are

$$
B_\alpha=\{p\in X^2:\|p\|_2\leq\alpha\},\qquad
C=A^*B_\alpha.
$$

The set $C$ is nonempty, convex and compact, hence closed, because it is a linear [image signal](../../../../../image-signal.md) of a compact ball in finite dimensions. [Euclidean norm duality](../../../../../euclidean-norm-duality.md) gives

$$
\alpha\|Au\|_2=\sup_{p\in B_\alpha}\langle Au,p\rangle
=\sup_{w\in C}\langle u,w\rangle=\sigma_C(u),
$$

the [support function](../../../../../support-function.md) of $C$.

The [metric projection onto a closed convex set](../../../../../euclidean-projection-onto-a-convex-set.md) $w=P_Cg$ uniquely minimizes $\|g-w\|^2$ over $C$. Its [variational characterization of convex projection](../../../../../variational-characterization-of-convex-projection.md) says

$$
\langle g-w,z-w\rangle\leq0\quad(z\in C).
$$

Put $u_*=g-w$. This inequality says precisely that $\sigma_C(u_*)=\langle u_*,w\rangle$. For any $v\in X$, the primal energy satisfies

$$
\sigma_C(v)+\frac12\|v-g\|^2
\geq\langle v,w\rangle+\frac12\|v-g\|^2.
$$

Completing the square shows that the right side is uniquely minimized by $v=g-w$. At that point the inequality is equality, so

$$
\boxed{u_*=g-P_Cg,\qquad C=\nabla^*B_\alpha.}
$$

This also follows from the [proximal operator of a support function](../../../../../proximal-operator-of-a-support-function.md) and [Moreau decomposition](../../../../../moreau-decomposition.md): the [convex conjugate](../../../../../convex-conjugate.md) of $\sigma_C$ is the [indicator functional of a constraint set](../../../../../indicator-functional-of-a-constraint-set.md) for $C$. The squared fidelity is [strictly convex](../../../../../strictly-convex-function.md) and coercive, so the primal [minimizer](../../../../../global-minimizer.md) exists and is unique.

The [convex projection](../../../../../euclidean-projection-onto-a-convex-set.md) in this formula is the removed component $g-u_*$, not generally $u_*$ itself. A metric [convex projection](../../../../../euclidean-projection-onto-a-convex-set.md) onto one fixed closed [convex set](../../../../../convex-set.md) is idempotent. On a [right singular vector](../../../../../right-singular-vector.md) direction with positive singular value of any nonzero $A$, this denoising map reduces to [soft thresholding](../../../../../soft-thresholding.md) with a positive threshold, and applying it twice shrinks again. It therefore cannot be such a [convex projection](../../../../../euclidean-projection-onto-a-convex-set.md) for all data. This qualifies the printed [convex projection](../../../../../euclidean-projection-onto-a-convex-set.md) wording while giving the required [global gradient-norm projection residual](../../../../../global-gradient-norm-projection-residual.md).

Compute $P_Cg$ by solving the convex dual least-squares problem

$$
\min_{p\in B_\alpha}f(p),\qquad
f(p)=\frac12\|g-A^*p\|^2.
$$

Its [gradient](../../../../../gradient.md) is $\nabla f(p)=A(A^*p-g)$ and has [Lipschitz constant](../../../../../lipschitz-constant.md) $L=\|A\|^2$. [Projected gradient descent](../../../../../projected-gradient-descent.md) gives

$$
\boxed{p^{n+1}=P_{B_\alpha}\big[p^n+\tau A(g-A^*p^n)\big],\qquad
P_{B_\alpha}(r)=\frac{r}{\max(1,\|r\|_2/\alpha)}.}
$$

For fixed $0<\tau<2/L$, the finite-dimensional projected-gradient convergence theorem ensures that $p^n$ converges to a dual [minimizer](../../../../../global-minimizer.md). Reconstruct $u^n=g-A^*p^n$; its limit is the unique primal solution even if dual [minimizers](../../../../../global-minimizer.md) are nonunique. If $A=0$, the primal solution is simply $g$ and no iteration is needed. For unit-grid forward differences with periodic or zero-difference boundaries, $\|A\|^2\leq8$, so $0<\tau<1/4$ is sufficient. Grid-spacing factors or other boundary stencils change this bound.

The normalization here is global. If a pixelwise sum of [gradient](../../../../../gradient.md) lengths had instead been intended, the dual feasible set would be a product of pixelwise balls and [convex projection](../../../../../euclidean-projection-onto-a-convex-set.md) would normalize each block separately; it is a different regularizer and should not be silently substituted.

For the [discrete Hessian-norm denoising](../../../../../discrete-hessian-norm-denoising.md) variant, write $H=\nabla^2:X\to X^4$ and use

$$
\boxed{C_H=H^*\{p\in X^4:\|p\|_2\leq\alpha\},\qquad
u_*=g-P_{C_H}g.}
$$

This is again a compact convex [image signal](../../../../../image-signal.md) of a Euclidean ball, now under the second-difference adjoint. In suitable conventions $H^*$ is a discrete double divergence, but its exact boundary adjoint is what defines the set. It lies in $(\ker H)^\perp$, so components in $\ker H$ are preserved by denoising. Interior second [derivatives](../../../../../derivative.md) annihilate affine [image signals](../../../../../image-signal.md); whether all such [image signals](../../../../../image-signal.md) remain in the kernel depends on the boundary convention. With a pixelwise Hessian [norm](../../../../../norm.md), the corresponding balls would instead be four-component blocks.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

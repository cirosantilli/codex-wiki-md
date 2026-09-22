<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $F[A]=\partial_\mu A_\mu+iA_\mu A_\mu$ and choose the [U(1) gauge symmetry](../../../../../../u-1-gauge-symmetry.md) convention $A_\mu\mapsto A_\mu+\partial_\mu\alpha$. Its infinitesimal variation is

$$
\delta_\alpha F[A]=M_A\alpha,\qquad M_A=\partial^2+2iA_\mu\partial_\mu.
$$

A formal [BRST symmetry](../../../../../../brst-symmetry.md) construction uses $sA_\mu=\partial_\mu c$, $sc=0$, $s\bar c=ih$, $sh=0$ and the [gauge-fixing fermion](../../../../../../gauge-fixing-fermion.md) $\Psi=\int\bar c(F-i\xi h/2)\,d^4x$. Acting with the odd differential gives

$$
\boxed{S_{\mathrm{gf+gh}}=s\Psi=\int d^4x\left[ihF[A]+\frac\xi2h^2+\bar c\,\mathcal O_Ac\right],\qquad\mathcal O_A=-\partial^2-2iA\cdot\partial.}
$$

For a real admissible gauge functional, integration over $h$ gives $F^2/(2\xi)$ in the [Euclidean action](../../../../../../euclidean-action.md), and $\xi\to0$ imposes the gauge condition. Overall constant phases in the [Faddeev-Popov determinant](../../../../../../faddeev-popov-determinant.md) can be absorbed in the measure convention. Here [nonlinear Abelian gauge fixing](../../../../../../nonlinear-abelian-gauge-fixing.md) makes $\mathcal O_A$ depend on $A$. The action for the [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md) contains the interaction $-2i\bar cA_\mu\partial_\mu c$, so the [Faddeev-Popov ghost fields](../../../../../../faddeev-popov-ghost.md) cannot be discarded as in a linear Abelian gauge, even though the $U(1)$ [Adjoint representation](../../../../../../adjoint-representation-of-a-lie-algebra.md) is trivial.

There is a genuine [reality obstruction for a complex Euclidean gauge condition](../../../../../../reality-obstruction-for-a-complex-euclidean-gauge-condition.md) in the source. For a Hermitian $U(1)$ [gauge field](../../../../../../gauge-field.md), each Euclidean component $A_\mu$ is real. The real and imaginary parts of $F=0$ separately require $\partial\cdot A=0$ and $\sum_\mu A_\mu^2=0$, hence $A=0$. For example $A_2=Bx_1$, with other components zero and $B\ne0$, has curvature $F_{12}=B$; no [gauge transformation](../../../../../../gauge-transformation.md) can put it on this slice because curvature is gauge invariant. Thus the stated condition is not a [gauge fixing](../../../../../../gauge-fixing.md) of general real Euclidean configurations. The boxed action is the intended formal complex-gauge construction. A legitimate complexified contour prescription would be additional data, not an ordinary real delta-functional enforcing this printed condition.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

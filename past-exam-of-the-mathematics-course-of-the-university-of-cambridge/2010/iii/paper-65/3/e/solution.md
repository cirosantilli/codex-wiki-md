<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First derive the formal [turbulent plane jet similarity](../../../../../../turbulent-plane-jet-similarity.md) equations, then check the printed edge conditions. Define a [streamfunction](../../../../../../stream-function.md) by $U=\psi_y$, $V=-\psi_x$, so mean [incompressibility](../../../../../../incompressible-flow.md) is automatic. Momentum conservation gives $U_c^2\delta\sim M_0$. With $l=C_1|y|$, the closure balance $U_c^2/x\sim C_1^2U_c^2/\delta$ gives $\delta\propto x$. Hence $U_c\propto M_0^{1/2}x^{-1/2}$ and the consistent [self-similar ansatz](../../../../../../self-similar-ansatz.md) is

$$
\boxed{\psi=M_0^{1/2}x^{1/2}f(\eta),\qquad\eta=y/x.}
$$

An odd $f$ gives symmetric $U$ and antisymmetric $V$. Direct differentiation gives

$$
U=M_0^{1/2}x^{-1/2}f',\qquad
V=M_0^{1/2}x^{-1/2}(\eta f'-f/2),\qquad
U_y=M_0^{1/2}x^{-3/2}f''.
$$

The advection and [Reynolds stress](../../../../../../reynolds-stress.md) terms become

$$
UU_x+VU_y=-\frac{M_0}{2x^2}\{(f')^2+ff''\},\qquad
-\partial_y\overline{\hat u\hat v}
=-\frac{C_1^2M_0}{x^2}\operatorname{sgn}(\eta)[\eta^2(f'')^2]'.
$$

Thus the two required consistency equations, the first for $\eta>0$ and the second for a symmetric finite-width profile, are

$$
\boxed{\frac12(ff')'=C_1^2[\eta^2(f'')^2]',\qquad
2\int_0^{\eta_w}(f')^2\,d\eta=1.}
$$

The second is momentum normalization; it is the equation referenced as (2) in the PDF, although its display in part (d) has no printed number. Use an infinite upper limit for a decaying profile of infinite support. Symmetry sets $f(0)=0$. A finite centreline velocity and continuous zero centreline stress give the integrated first equation

$$
\boxed{ff'=2C_1^2\eta^2(f'')^2.}
$$

These equations establish the similarity reduction. They also give a direct [finite-edge stress condition for a mixing-length jet](../../../../../../finite-edge-stress-condition-for-a-mixing-length-jet.md). At a finite edge $\eta_w>0$, $U=0$ requires $f'(\eta_w)=0$. For finite $f(\eta_w)$, the integrated equation forces $f''(\eta_w)=0$. A nontrivial decreasing velocity profile has nonzero shear somewhere inside, so zero edge shear cannot be its maximum. Allowing a one-sided nonzero edge shear instead produces nonzero edge stress and an unbalanced jump in the conservative momentum equation.

For a concrete diagnostic, take $f'=1-\eta^2$ on $0\leq\eta\leq1$, so $f=\eta-\eta^3/3$. It has zero edge velocity and its largest one-sided shear magnitude at the edge, matching that descriptive condition. Yet at $\eta=1$ the integrated equation has left-hand side zero and right-hand side $8C_1^2>0$: such a profile is not a solution of the stated momentum closure.

The centreline is also problematic for a smooth interpretation. If $f'(0)=a>0$, then $f\sim a\eta$, and the decreasing branch of the integrated equation gives

$$
f''\sim-\frac{a}{\sqrt2C_1\sqrt\eta},\qquad
f'=a-\frac{\sqrt2a}{C_1}\sqrt\eta+o(\sqrt\eta).
$$

A continuous formal profile can have this cusp, but it is not a differentiable symmetric velocity field, and molecular diffusion cannot be neglected uniformly in that core. Therefore **there is no nontrivial regular similarity solution satisfying all the printed edge requirements**. The boxed consistency equations are valid; the additional coincidence of a zero-velocity edge with maximum shear is not. A consistent jet model must relax that edge definition and regularize the core or use a different [mixing length](../../../../../../mixing-length.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

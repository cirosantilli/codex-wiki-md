<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $r=x-\bar x$, $A(t)=\int_0^t\alpha(s)ds$, and use the usual reduced rigid-recoil representation $h=Z+r\theta-\alpha r^2$, with zero initial recoil and a smooth stroke returning $\alpha$ and $\dot\alpha$ to zero. For this representation,

$$
\gamma=Z+U\int_0^t\theta(s)ds,\qquad
w=\dot\gamma+r\dot\theta-\dot\alpha r^2-2U\alpha r.
$$

Define the fluid impulse and its first moment by

$$
Q=M_0\dot\gamma+M_1\dot\theta-M_2\dot\alpha-2UM_1\alpha,\qquad
P=M_1\dot\gamma+M_2\dot\theta-M_3\dot\alpha-2UM_2\alpha.
$$

The [force](../../../../../../force.md) law from part (i) gives, by [integration by parts](../../../../../../integration-by-parts.md),

$$
\int_0^L F_zdx=\dot Q+U[mw]_0^L,\qquad
\int_0^L rF_zdx=\dot P+U[rmw]_0^L-UQ.
$$

These are the [endpoint momentum flux in elongated-body recoil](../../../../../../endpoint-momentum-flux-in-elongated-body-recoil.md). Put

$$
B_j=[m(x)r^j]_0^L,\qquad j=0,1,2,3.
$$

The endpoint quantities are needed in addition to the integrals $M_j$ unless further end-shape assumptions are made. Lateral [force](../../../../../../force.md) and yaw [torque](../../../../../../torque.md) balance are

$$
M_b\ddot Z=-\dot Q-U[mw]_0^L,\qquad
I_b\ddot\theta=-\dot P-U[rmw]_0^L+UQ.
$$

Expanding gives the requested simultaneous second-order equations, with the retained endpoint fluxes:

$$
\boxed{\begin{aligned}
(M_b+M_0)\ddot Z+M_1\ddot\theta+UB_0\dot Z
+U(M_0+B_1)\dot\theta+U^2B_0\theta
&=M_2\ddot\alpha+U(2M_1+B_2)\dot\alpha+2U^2B_1\alpha,\\
M_1\ddot Z+(I_b+M_2)\ddot\theta+U(B_1-M_0)\dot Z
+UB_2\dot\theta+U^2(B_1-M_0)\theta
&=M_3\ddot\alpha+U(M_2+B_3)\dot\alpha+2U^2(B_2-M_1)\alpha.
\end{aligned}}
$$

Substituting $\ddot Z=\ddot\gamma-U\dot\theta$ and integrating once from the initially straight, unrecoiling state yields

$$
\boxed{\begin{aligned}
(M_b+M_0)\dot\gamma+M_1\dot\theta+UB_0\gamma+U(B_1-M_b)\theta
&=M_2\dot\alpha+U(2M_1+B_2)\alpha+2U^2B_1A,\\
M_1\dot\gamma+(I_b+M_2)\dot\theta+U(B_1-M_0)\gamma+U(B_2-M_1)\theta
&=M_3\dot\alpha+U(M_2+B_3)\alpha+2U^2(B_2-M_1)A.
\end{aligned}}
$$

These are first-order coupled equations for $\gamma,\theta$ with known forcing.

The claimed mass-independent final angle requires a qualification. Let

$$
\mathsf M=\begin{pmatrix}M_b+M_0&M_1\\M_1&I_b+M_2\end{pmatrix},\qquad
\mathsf K=\begin{pmatrix}B_0&B_1-M_b\\B_1-M_0&B_2-M_1\end{pmatrix}.
$$

After the stroke, $\alpha=\dot\alpha=0$ and $A=A_T=\int_0^T\alpha dt$. If the post-stroke dynamics are stable, the first-order system relaxes to

$$
\mathsf K\begin{pmatrix}\gamma_\infty\\\theta_\infty\end{pmatrix}
=2UA_T\begin{pmatrix}B_1\\B_2-M_1\end{pmatrix}.
$$

Let $C=B_0(B_2-M_1)-B_1(B_1-M_0)$. Solving this two-by-two system gives

$$
\boxed{\theta_\infty=2UA_T\frac{C}{C+M_b(B_1-M_0)},\qquad
\gamma_\infty=2UA_T\frac{M_b(B_2-M_1)}{C+M_b(B_1-M_0)}.}
$$

This is [quadratic-bend turning with finite body mass](../../../../../../quadratic-bend-turning-with-finite-body-mass.md). At the limiting state $\dot\theta=\dot\gamma=0$, so $\dot Z=-U\theta_\infty$. The forward [velocity](../../../../../../velocity.md) is $-U$ in the chosen $x$ direction, and its lateral component has precisely the body's slope: the fish glides parallel to itself. The angle is generally reached after a relaxation transient, not necessarily immediately at $t=T$.

The advertised result is obtained in the thin-body approximation that neglects $M_b$ relative to fluid [added mass](../../../../../../added-mass.md), or in the special geometry $B_1=M_0$:

$$
\boxed{\theta_\infty=2U\int_0^T\alpha(t)dt.}
$$

For example, take negligible nose [added mass](../../../../../../added-mass.md) and nonzero tail [added mass](../../../../../../added-mass.md) $m_T$, so $B_j=m_T(L-\bar x)^j$. In the zero-body-mass approximation, the post-stroke equations for $(\gamma,\theta-2UA_T)$ are homogeneous. The inertia [matrix](../../../../../../matrix.md) is positive definite by [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), and

$$
\det\mathsf K=m_T\int_0^Lm(x)(L-x)dx>0,\qquad
\operatorname{tr}(\mathsf M^{-1}\mathsf K)
=\frac{m_T[I_b+\int_0^Lm(x)(L-x)^2dx]}{\det\mathsf M}>0.
$$

The two [eigenvalues](../../../../../../eigenvalue.md) of $\mathsf M^{-1}\mathsf K$ therefore have positive real parts: their sum and product are positive, whether they are real or conjugate. For $U>0$ the transient decays, proving parallel gliding and the displayed turn in this approximation.

With finite $M_b$, the angle is not a consequence of the printed [force](../../../../../../force.md) law for arbitrary $m(x)$. A concrete stable counterexample uses $L=1$, $\bar x=1/2$, and $m(x)=m_*x^2$. Then $M_0=m_*/3$, $M_1=m_*/12$, $B_0=m_*$, $B_1=m_*/2$, $B_2=m_*/4$, and $C=m_*^2/12$. Hence

$$
\theta_\infty=\frac{2UA_T}{1+2M_b/m_*},
$$

which differs from $2UA_T$ for positive body [mass](../../../../../../mass.md). This example has positive [determinant](../../../../../../determinant.md) and positive [matrix trace](../../../../../../matrix-trace.md) of the relaxation [matrix](../../../../../../matrix.md). Another immediate check is that if both endpoint added masses vanish, integrating the [force](../../../../../../force.md) law conserves total lateral [momentum](../../../../../../momentum.md). A finite-mass fish cannot then end with $w=0$ and a nonzero new transverse [velocity](../../../../../../velocity.md). Thus endpoint and inertia assumptions cannot silently be omitted.

If $Z$ is literally the [centre of mass](../../../../../../center-of-mass.md) position of a deforming body, use a mass-centered deformation rather than the raw quadratic. For body [mass density](../../../../../../density.md) $\mu_b(x)$, its mean is $-\alpha J_2/M_b$, with $J_2=\int\mu_b r^2dx$; in the slender approximation $J_2=I_b$. The reference translation above is then $Z_r=Z+\alpha J_2/M_b$. Likewise the active [angular momentum](../../../../../../angular-momentum.md) contains $-\dot\alpha J_3$, where $J_3=\int\mu_b r^3dx$, which vanishes for symmetric [mass](../../../../../../mass.md) distribution. These corrections modify [derivative](../../../../../../derivative.md) forcing during the stroke. Since the shape and its time [derivative](../../../../../../derivative.md) return to zero, they do not remove the finite-body-mass qualification of the final impulse relation.

The principal physical limitations are small slopes and small total turning angle, prescribed approximately constant forward speed, slowly varying slender geometry, and neglected [viscosity](../../../../../../dynamic-viscosity.md), separation and detailed three-dimensional wake interactions. Fast large-amplitude C-starts need more than this linear theory. Neglecting body [mass](../../../../../../mass.md) is most reasonable for a laterally thin body whose crossflow [added mass](../../../../../../added-mass.md) greatly exceeds its displaced [mass](../../../../../../mass.md). Stable relaxation also requires an appropriate tail/end geometry; it is not guaranteed for every added-mass profile.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

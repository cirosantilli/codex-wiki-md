<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [basic reproduction number](../../../../../basic-reproduction-number.md) is the [expected value](../../../../../expected-value.md) of secondary infections caused by one typical infectious individual introduced into an otherwise susceptible population. For a heterogeneous model it is the dominant [eigenvalue](../../../../../eigenvalue.md) of the next-generation operator, so the appropriate infected-type distribution is part of “typical.” A small introduction grows when $\mathcal R_0>1$ and decays when $\mathcal R_0<1$, under the usual linear invasion assumptions.

The asymptotic susceptible level depends on the model. In a homogeneous [SIS model](../../../../../sis-model.md) with transmission rate $\beta$ and recovery rate $\gamma$, the positive endemic [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) has $S_*=1/\mathcal R_0$ when $\mathcal R_0=\beta/\gamma>1$. In a closed [SIR model](../../../../../sir-model.md), however, the [final size relation for an epidemic](../../../../../final-size-relation-for-an-epidemic.md) is

$$
\log(S_\infty/S_0)=-\mathcal R_0(R_\infty-R_0^{\rm recovered}).
$$

For an infinitesimal seed in a wholly susceptible population this becomes $-\log S_\infty=\mathcal R_0(1-S_\infty)$. The [epidemic](../../../../../epidemic.md) peak occurs at $S=1/\mathcal R_0$, and a nontrivial outbreak leaves $S_\infty<1/\mathcal R_0$. Thus **$1/\mathcal R_0$ is an endemic or instantaneous invasion threshold, not a universal final susceptible fraction.**

For cooperative infections, let $s,x,y,z$ be the fractions carrying neither infection, only $A$, only $B$, and both, with sum one. Let $\lambda_A=\beta_A(x+z)$, $\lambda_B=\beta_B(y+z)$, assume each infection independently recovers at rate $\gamma$, and multiply susceptibility to the second infection by $q>1$. One suitable pair of [SIS models](../../../../../sis-model.md) is

$$
\begin{aligned}
\dot x&=\lambda_As-q\lambda_Bx-\gamma x+\gamma z,\\
\dot y&=\lambda_Bs-q\lambda_Ay-\gamma y+\gamma z,\\
\dot z&=q\lambda_Bx+q\lambda_Ay-2\gamma z,\\
\dot s&=-(\lambda_A+\lambda_B)s+\gamma(x+y).
\end{aligned}
$$

Recovery of one infection from $z$ leads to the other single-infection class, not directly to $s$. The [probability simplex](../../../../../probability-simplex.md) is invariant. At the disease-free [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) the [eigenvalues](../../../../../eigenvalue.md) are $\beta_A-\gamma$, $\beta_B-\gamma$ and $-2\gamma$. Therefore failure of both isolated and low-density invasion requires $\mathcal R_A=\beta_A/\gamma<1$, $\mathcal R_B=\beta_B/\gamma<1$. Enhancement of secondary susceptibility does not alter these linear thresholds because coinfection is second order at introduction.

For completeness, a joint positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) must have

$$
x=\frac{\mathcal R_B^{-1}-s}{q},\qquad
y=\frac{\mathcal R_A^{-1}-s}{q},\qquad
z=1-s-x-y,
$$

and

$$
(q-1)s^2-qs+\frac1{\mathcal R_A\mathcal R_B}=0.
$$

To obtain these, divide the [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) equations for total $A$ and total $B$ prevalence by their positive prevalences, yielding $s+qy=\mathcal R_A^{-1}$ and $s+qx=\mathcal R_B^{-1}$. Substitution into the $s$ balance gives the quadratic. Its discriminant must be nonnegative and the resulting $x,y,z$ positive. These conditions test [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) feasibility for unequal rates; stability must also be checked rather than inferred from the mere presence of a root.

A fully explicit [Allee effect](../../../../../allee-effect.md) results in the symmetric permitted case $\beta_A=\beta_B=\beta$, $\mathcal R=\beta/\gamma$. The joint [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) have

$$
s_\pm=\frac{q\pm\sqrt{q^2-4(q-1)/\mathcal R^2}}{2(q-1)},\qquad
x=y=\frac{\mathcal R^{-1}-s_\pm}{q}.
$$

Two feasible positive [equilibria](../../../../../equilibrium-point-of-a-dynamical-system.md) coexist with the stable disease-free state exactly in the strict range

$$
\boxed{q>2,\qquad \frac{2\sqrt{q-1}}q<\mathcal R<1.}
$$

Indeed at the fold the two roots coalesce, and at $\mathcal R=1$ the smaller-prevalence branch reaches the disease-free boundary. For $q\leq2$, roots at $\mathcal R<1$ do not give positive singly infected fractions. Strict inequalities exclude these marginal endpoints.

Here is the stability check underlying the [cooperative SIS coinfection threshold](../../../../../cooperative-sis-coinfection-threshold.md). On the symmetric subspace put $v=x+z=y+z$ and $c=z$. Then

$$
\dot v=\gamma v\{\mathcal R[1+(q-2)v-(q-1)c]-1\},\qquad
\dot c=2\gamma[q\mathcal Rv(v-c)-c].
$$

At a positive [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md) $c=q\mathcal Rv^2/(1+q\mathcal Rv)$. Its two-dimensional [Jacobian matrix](../../../../../jacobian-matrix.md) has

$$
\operatorname{tr}J=-\gamma[\mathcal Rv(q+2)+2],\qquad
\det J=\frac{2\gamma^2\mathcal Rv}{1+q\mathcal Rv}\bigl[(1+q\mathcal Rv)^2-(q-1)\bigr].
$$

The higher-prevalence branch has positive [determinant](../../../../../determinant.md) and negative [trace](../../../../../matrix-trace.md), while the lower-prevalence branch is a [saddle equilibrium](../../../../../saddle-equilibrium.md). The remaining antisymmetric mode, from $x-y$, has [eigenvalue](../../../../../eigenvalue.md) $-q\beta v<0$. Thus the smaller susceptible root $s_-$ is a stable joint endemic [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), separated from the stable zero state by a finite seeding threshold. Neither infection can persist alone in this range. **Strong cooperation can sustain both infections after a sufficiently large joint introduction even though neither invades from rarity.** The numerical condition belongs to the specified secondary-susceptibility model; alternative cooperation mechanisms need their own threshold calculation.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

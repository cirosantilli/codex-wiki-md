<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First there is a necessary coordinate qualification. With the literal $z$ action obtained in part (c), the temporal weights are $-1,+1$ and reflection is conjugation followed by exchange. A linear term with $(\mu+i\omega)$ in both equations fails reflection equivariance for $\omega\ne0$, since conjugation changes the sign of $i\omega$. The proposed first-component [monomial](../../../../../../monomial.md) $\bar z_1z_2^2$ also has temporal weight $+3$, rather than $-1$. Thus the displayed equations cannot be proved in those literal coordinates. They are the correct [dihedral fourfold Hopf normal form](../../../../../../dihedral-fourfold-hopf-normal-form.md) in the common-phase Hopf coordinates $(q_1,q_2)=(z_1,\bar z_2)$.

In these coordinates the temporal circle imposes total phase weight one on every vector-field [monomial](../../../../../../monomial.md). There are no quadratic [monomials](../../../../../../monomial.md) with that weight. A cubic [monomial](../../../../../../monomial.md) has two unbarred factors and one barred factor. For the first component, rotation by $\rho$ must multiply the [monomial](../../../../../../monomial.md) by $i$. Inspecting the six phase-compatible [monomials](../../../../../../monomial.md) leaves precisely

$$
q_1^2\bar q_1=q_1|q_1|^2,\qquad q_1q_2\bar q_2=q_1|q_2|^2,\qquad q_2^2\bar q_1.
$$

The excluded three [monomials](../../../../../../monomial.md) multiply by $-i$ instead. Reflection swaps the components, so their coefficients must be the same after swapping indices. The linear part is a scalar complex multiple by absolute irreducibility. Orient the Hopf parameter to write it as $\mu+i\omega$, and name the cubic coefficients $-a,-b,-c$, where $a,b,c$ are generally complex. This proves

$$
\boxed{\begin{aligned}
\dot q_1&=(\mu+i\omega)q_1-aq_1|q_1|^2-bq_1|q_2|^2-c\bar q_1q_2^2,\\
\dot q_2&=(\mu+i\omega)q_2-aq_2|q_2|^2-bq_2|q_1|^2-c\bar q_2q_1^2.
\end{aligned}}
$$

These are cubic amplitude [normal forms of a dynamical system](../../../../../../normal-form-dynamical-systems.md), after the usual symmetry-compatible Hopf normalization. Returning to literal $z$ coordinates conjugates the second equation: its linear coefficient is $\mu-i\omega$, its cubic coefficients are $\bar a,\bar b,\bar c$, and the first coupling is $-c\bar z_1\bar z_2^2$. That corrected form respects every printed generator.

On the three [complex axial isotropy subgroup](../../../../../../complex-axial-isotropy-subgroup.md) fixed spaces, substitute $q_1=Re^{i\Omega t}$ and $q_2=0,q_1,iq_1$. The radial equations are $\dot R=R(\mu-A_jR^2)$, with

$$
A_R=\operatorname{Re}a,\qquad A_A=\operatorname{Re}(a+b+c),\qquad
A_D=\operatorname{Re}(a+b-c).
$$

Therefore the leading component amplitudes are

$$
\boxed{R_R^2=\frac\mu{\operatorname{Re}a},\qquad
R_A^2=\frac\mu{\operatorname{Re}(a+b+c)},\qquad
R_D^2=\frac\mu{\operatorname{Re}(a+b-c)}.}
$$

Each expression applies on the parameter side where it is positive, with its denominator nonzero for a nondegenerate branch. The frequencies are $\Omega_j=\omega-\operatorname{Im}(a_j)R_j^2$, with $a_j=a,a+b+c,a+b-c$. The denominators are generically distinct, so coexisting branches generically have different component amplitudes. If the amplitude is instead measured by the original real-space norm, the identity $|w_1|^2+|w_2|^2=2(|q_1|^2+|q_2|^2)$ gives squared amplitudes $2R_R^2$, $4R_A^2$, and $4R_D^2$, again generically distinct. Equalities require special coefficient relations, rather than symmetry forcing them.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

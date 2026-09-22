<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The specific [Helmholtz free energy](../../../../../../helmholtz-free-energy.md) $\psi=U-\theta\eta$ satisfies $d\psi=\rho_0^{-1}P_{Ii}\,dF_{iI}-\eta\,d\theta-\rho_0^{-1}f_r\,d\xi_r$. For the [multiplicative decomposition of the deformation gradient](../../../../../../multiplicative-decomposition-of-the-deformation-gradient.md) $F=F_*A$, adopt $P^*_{Ji}=\rho_0\partial\psi/\partial(F_*)_{iJ}$, consistently with the material-first [nominal stress tensor](../../../../../../nominal-stress-tensor.md). Differentiating $F_*=FA^{-1}$ gives

$$
dF_*=dF\,A^{-1}-F_*\,dA\,A^{-1}.
$$

Consequently

$$
P_{Ii}=(A^{-1})_{IJ}P^*_{Ji},\qquad Q_{IJ}=P_{Ii}(F_*)_{iJ},
$$

or

$$
\boxed{P=A^{-1}P^*,\qquad Q=A^{-1}P^*F_*=PF_*.}
$$

These relations follow from the [chain rule](../../../../../../chain-rule.md); the transpose convention matters.

Differentiating the [dissipation potential](../../../../../../dissipation-potential.md), with the [Frobenius norm](../../../../../../frobenius-norm.md) of $Q$, gives

$$
\dot A_{JI}=\alpha\|Q\|^{n-1}Q_{IJ}-\frac{A_{JI}}{\tau}.
$$

An [integrating factor](../../../../../../integrating-factor.md) yields the [exponential memory from tensor relaxation](../../../../../../exponential-memory-from-tensor-relaxation.md):

$$
\boxed{A(t)=e^{-t/\tau}A(0)+\alpha\int_0^t e^{-(t-s)/\tau}\|Q(s)\|^{n-1}Q(s)^T\,ds.}
$$

For $n>0$, the driving term is continuously zero at $Q=0$.

Taking the product $T=PF$ explicitly defined in the question, $F=F_*A$ gives $T=QA$, and hence its requested history functional is

$$
\boxed{T_{\rm printed}(t)=Q(t)\left[e^{-t/\tau}A(0)+\alpha\int_0^t e^{-(t-s)/\tau}\|Q(s)\|^{n-1}Q(s)^T\,ds\right].}
$$

There is a naming error in the PDF: with its $P_{Ii}$ convention, the actual [second Piola-Kirchhoff stress tensor](../../../../../../second-piola-kirchhoff-stress-tensor.md) is $S=PF^{-T}$, while $PF=SC$ is the transpose of the [Mandel stress tensor](../../../../../../mandel-stress-tensor.md), where $C=F^TF$. Thus $S=QA\,C^{-1}$ if that stress measure is required. This agrees with the stress push-forward used in Question 5; the printed product is fully determined by the history above, whereas recovering $S$ also requires the deformation or an invertible elastic constitutive relation.

The [multiplicative decomposition of the deformation gradient](../../../../../../multiplicative-decomposition-of-the-deformation-gradient.md) is used on histories where $A$ stays invertible. Thermodynamic admissibility additionally requires $\operatorname{tr}(Q\dot A)=\alpha\|Q\|^{n+1}-\operatorname{tr}(AQ)/\tau\ge0$: positivity of the constants alone does not ensure this for arbitrary prescribed histories.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

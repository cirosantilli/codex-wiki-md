<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For [Kraus operators](../../../../../../kraus-operator.md) $A_j$, the [Kraus formula for entanglement fidelity](../../../../../../kraus-formula-for-entanglement-fidelity.md) is

$$
F_e(\rho,\Lambda)=\sum_j|\operatorname{Tr}(\rho A_j)|^2.
$$

Indeed each Kraus contribution to the purified-state overlap is $|\langle\Psi|(I\otimes A_j)|\Psi\rangle|^2$, and the expectation in a purification is $\operatorname{Tr}(\rho A_j)$. In this case,

$$
\operatorname{Tr}(\rho A_1)=\frac{1+s_z+\sqrt{1-p}(1-s_z)}2,\qquad
\operatorname{Tr}(\rho A_2)=\frac{\sqrt p}{2}(s_x+is_y).
$$

The [entanglement fidelity of amplitude damping](../../../../../../entanglement-fidelity-of-amplitude-damping.md) is thus

$$
\boxed{F_e(\rho,\Lambda)=\frac14\left[1+s_z+\sqrt{1-p}(1-s_z)\right]^2
+\frac p4(s_x^2+s_y^2).}
$$

For $p=0$, this is one. For a ground-state input it is one for every $p$, whereas for an excited-state input it is $1-p$. These checks agree with the physical relaxation mechanism.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

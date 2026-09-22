<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Every positive-energy [Dirac spinor](../../../../dirac-spinor.md) obeys $(\not p-m)u^s(\mathbf p)=0$. Therefore the [fermion spin sum](../../../../fermion-spin-sum.md) satisfies

$$
(\not p-m)P=\sum_s[(\not p-m)u^s]\bar u^s=0.
$$

Since $\bar u^s=u^{s\dagger}\gamma^0$ and $(\gamma^0)^2=I$, the [trace](../../../../matrix-trace.md) of each outer product is its contracted scalar. The prescribed normalization and the two [spin](../../../../spin.md) states yield

$$
\boxed{\operatorname{tr}(P\gamma^0)=\sum_su^{s\dagger}u^s=2(2E_p)=4E_p.}
$$

Now make exactly the stated [polynomial](../../../../polynomial-split.md) assumption and apply [polynomial reduction of a slashed vector](../../../../polynomial-reduction-of-a-slashed-vector.md). By [a](../a.md), on the [mass shell](../../../../mass-shell.md) $p^2=m^2$ write $P=A\not p+BI$. Then

$$
0=(\not p-m)P=(Am^2-mB)I+(B-mA)\not p.
$$

The [matrices](../../../../matrix.md) $I$ and $\not p$ are linearly independent for a physical nonzero $p$, so $B=mA$. The [gamma matrix trace identities](../../../../gamma-matrix-trace-identities.md), $\operatorname{tr}\gamma^0=0$ and $\operatorname{tr}(\gamma^\mu\gamma^0)=4\eta^{\mu0}$, give

$$
4E_p=\operatorname{tr}[A(\not p+m)\gamma^0]=4AE_p.
$$

Thus $A=1$ and

$$
\boxed{P(\mathbf p)=\not p+m.}
$$

No explicit representation of the [Dirac spinors](../../../../dirac-spinor.md) has been used. The same reasoning covers $m=0$ provided $p^0>0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

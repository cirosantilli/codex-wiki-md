<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [torsion-free connection](../../../../../../torsion-free-connection.md), the covariant Hessian of a scalar is symmetric, so $[\nabla_a,\nabla_b]f=0$. Moreover, a commutator of two covariant derivatives acts as a derivation on tensor products. Applying the [Leibniz rule](../../../../../../leibniz-rule.md) twice, the terms containing one derivative on each factor cancel between the two orders:

$$
[\nabla_a,\nabla_b](u\otimes v)=([\nabla_a,\nabla_b]u)\otimes v+u\otimes([\nabla_a,\nabla_b]v).
$$

Projecting with the parallel [symplectic form](../../../../../../symplectic-form.md) preserves this identity for the [chiral spinor curvature operator](../../../../../../chiral-spinor-curvature-operator.md). Since its scalar projection obeys $\Delta_{AB}f=0$, we obtain

$$
\boxed{\Delta_{AB}(f\alpha^C\beta^{C'})=f\left(\beta^{C'}\Delta_{AB}\alpha^C+\alpha^C\Delta_{AB}\beta^{C'}\right).}
$$

Thus the [chiral spinor curvature operator](../../../../../../chiral-spinor-curvature-operator.md) is algebraic over scalar functions even though its displayed expression uses second derivatives. If [torsion tensor](../../../../../../torsion-tensor.md) is allowed, $[\nabla_a,\nabla_b]f=-T^c{}_{ab}\partial_cf$ need not vanish, explaining why metric compatibility alone would not prove the claim.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

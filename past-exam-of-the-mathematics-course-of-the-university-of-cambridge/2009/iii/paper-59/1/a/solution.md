<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Levi-Civita connection](../../../../../../levi-civita-connection.md) interpretation of the curvature convention. Its [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) satisfies

$$
\boxed{R_{abcd}=-R_{bacd}=-R_{abdc},\qquad R_{abcd}=R_{cdab},\qquad R_{[abc]d}=0.}
$$

The first antisymmetry comes from the derivative commutator; the second comes from compatibility with the [metric tensor](../../../../../../metric-tensor.md). The cyclic identity is the [first Bianchi identity](../../../../../../first-bianchi-identity.md), and together these imply exchange symmetry of the two antisymmetric index pairs. Contracting gives the symmetric [Ricci tensor](../../../../../../ricci-tensor.md), $\boxed{R_{ab}=R_{ba}}$. The differential [Bianchi identity](../../../../../../bianchi-identity.md) is $\nabla_{[a}R_{bc]de}=0$.

There is a hypothesis qualification. A [metric connection](../../../../../../metric-connection.md) need not be a [torsion-free connection](../../../../../../torsion-free-connection.md). For a general such connection, the tensorial derivative commutator contains $-T^c{}_{ab}\nabla_c$ as well as curvature; pair exchange, the stated cyclic identity and Ricci symmetry need not hold. The printed pure-curvature commutator, and the scalar identity requested later, use the torsion-free interpretation. Under that intended interpretation all the boxed symmetries follow. They are not assertions about arbitrary metric-compatible connections with [torsion tensor](../../../../../../torsion-tensor.md).

For example, with a constant Minkowski metric a connection having only $\Gamma^1{}_{02}=1$ and $\Gamma^2{}_{01}=-1$ nonzero is metric compatible, since its connection matrix in direction zero is a spatial rotation. It has $T^1{}_{02}=1$. For the scalar $f=x^1$ the tensorial Hessian commutator is $[\nabla_0,\nabla_2]f=-1$, rather than zero. This explicitly demonstrates the missing zero-torsion condition used in the subsequent scalar proof.

## ↑ Ancestors (11)

1. [A](../a.md)
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

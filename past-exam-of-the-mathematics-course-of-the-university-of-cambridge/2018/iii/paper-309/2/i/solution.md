<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the curvature convention $[\nabla_b,\nabla_c]V^d=R^d{}_{abc}V^a$, consistent with the coordinate formula later in the paper. Choose [normal coordinates](../../../../../../normal-coordinates.md) at an arbitrary point $p$. The [Levi-Civita connection](../../../../../../levi-civita-connection.md) has $\Gamma^d{}_{ab}(p)=0$ and is torsion free, so $\Gamma^d{}_{ab}=\Gamma^d{}_{ba}$. At $p$,

$$
R^d{}_{abc}=\partial_b\Gamma^d{}_{ac}-\partial_c\Gamma^d{}_{ab}.
$$

Hence the cyclic sum is

$$
\begin{aligned}
R^d{}_{abc}+R^d{}_{bca}+R^d{}_{cab}
={}&\partial_b\Gamma^d{}_{ac}-\partial_c\Gamma^d{}_{ab}
+\partial_c\Gamma^d{}_{ba}-\partial_a\Gamma^d{}_{bc}\\
&+\partial_a\Gamma^d{}_{cb}-\partial_b\Gamma^d{}_{ca}=0.
\end{aligned}
$$

Each derivative cancels using symmetry of the two lower connection indices. Because the [Riemann curvature tensor](../../../../../../riemann-curvature-tensor.md) is antisymmetric in its last two indices, full antisymmetrization over $a,b,c$ equals one third of this cyclic sum. Thus

$$
\boxed{R^d{}_{[abc]}=0.}
$$

The statement is tensorial and $p$ was arbitrary, so it holds in all coordinates everywhere. This is the [first Bianchi identity](../../../../../../first-bianchi-identity.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

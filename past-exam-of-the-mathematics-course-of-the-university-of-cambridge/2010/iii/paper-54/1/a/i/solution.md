<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use signature $(-,+,+,+)$ and the [Riemann curvature tensor](../../../../../../../riemann-curvature-tensor.md) convention $[\nabla_a,\nabla_b]X^c=R^c{}_{dab}X^d$. Lower the index of the [Killing vector field](../../../../../../../killing-vector-field.md) and set $T_{abc}=\nabla_a\nabla_bV_c$. Differentiating the [Killing equation](../../../../../../../killing-equation.md) gives $T_{abc}=-T_{acb}$, while the [Ricci identity](../../../../../../../curvature-commutator-on-a-covariant-tensor.md) gives

$$
T_{abc}-T_{bac}=-R^d{}_{cab}V_d.
$$

Define $S_{abc}=R_{cbad}V^d$. The first-pair antisymmetry of the [Riemann curvature tensor](../../../../../../../riemann-curvature-tensor.md) gives $S_{abc}=-S_{acb}$. The pair symmetry and the [first Bianchi identity](../../../../../../../first-bianchi-identity.md) give

$$
S_{abc}-S_{bac}=(R_{cbad}-R_{cabd})V^d=-R_{dcab}V^d.
$$

Thus $D=T-S$ is symmetric in its first two indices and antisymmetric in its last two. These two symmetries force it to vanish:

$$
D_{abc}=D_{bac}=-D_{bca}=-D_{cba}=D_{cab}=D_{acb}=-D_{abc}.
$$

Consequently $T_{abc}=R_{cbad}V^d$. Raising $c$ using [metric compatibility](../../../../../../../metric-compatibility.md) proves the required [second covariant derivative of a Killing vector](../../../../../../../second-covariant-derivative-of-a-killing-vector.md):

$$
\boxed{\nabla_a\nabla_bV^c=R^c{}_{bad}V^d.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 54](../../../../paper-54-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

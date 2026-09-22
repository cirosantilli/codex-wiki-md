<h1 id="35a/solution">Solution</h1>

↑ **Parent:** [35A](../35a.md)

With the stated curvature convention, the [Ricci tensor](../../../../../ricci-tensor.md) is $R_{bd}=R^a{}_{bad}$ and the [scalar curvature](../../../../../scalar-curvature.md) is $R=g^{bd}R_{bd}$. Contract the differential [Bianchi identity](../../../../../bianchi-identity.md) once to give the divergence of the [Riemann tensor](../../../../../riemann-curvature-tensor.md), then again with the inverse metric. The curvature antisymmetries yield $\nabla^aR_{ab}-\nabla_bR+\nabla^aR_{ab}=0$, so $\nabla^aR_{ab}=\tfrac12\nabla_bR$.

The [Einstein field equations](../../../../../einstein-field-equations.md) are $G_{ab}+\Lambda g_{ab}=(8\pi G/c^4)T_{ab}$, with $G_{ab}=R_{ab}-\tfrac12Rg_{ab}$. The [contracted Bianchi identity](../../../../../contracted-bianchi-identity.md) makes the left side divergence-free, enforcing the local [stress-energy conservation](../../../../../stress-energy-conservation.md) law $\nabla^aT_{ab}=0$ and ensuring consistency of the matter equations with the gravitational constraints.

For a scalar, second covariant derivatives commute. Commuting a further derivative past the resulting covector introduces [Ricci curvature](../../../../../ricci-curvature.md), giving $\nabla^2\nabla_a\phi=\nabla_a\nabla^2\phi+R_{ab}\nabla^b\phi$.

Now $R_{ab}=\nabla_a\nabla_b\phi$ implies $R=\nabla^2\phi$. Taking its divergence and using that commutation formula gives $\tfrac12\nabla_bR=\nabla_bR+R_{ba}\nabla^a\phi$, hence $\nabla_bR=-2R_{ba}\nabla^a\phi$. Meanwhile $\nabla_b(\nabla_a\phi\nabla^a\phi)=2R_{ba}\nabla^a\phi$. Adding proves

$$
\boxed{R+\nabla_a\phi\nabla^a\phi=\text{constant on each connected component}.}
$$

In Riemannian signature this is the [steady gradient Ricci soliton scalar identity](../../../../../steady-gradient-ricci-soliton-scalar-identity.md), with soliton potential $f=-\phi$.

## ↑ Ancestors (10)

1. [35A](../35a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="17d/solution">Solution</h1>

↑ **Parent:** [17D](../17d.md)

Use the steady inviscid, hydrostatic, slowly varying channel approximation, without a [hydraulic jump](../../../../../hydraulic-jump.md). Conservation of volume flux per unit width gives $Q=u(x)h(x)=u_1h_1$. The free-surface [Bernoulli equation](../../../../../bernoulli-equation.md) is

$$
D(x)+h(x)+\frac{Q^2}{2gh(x)^2}=h_1+\frac{u_1^2}{2g}.
$$

Dividing by $h_1$ yields

$$
\boxed{\frac D{h_1}=1-\frac h{h_1}-\frac F2\left(\frac{h_1^2}{h^2}-1\right),\qquad F=\frac{u_1^2}{gh_1}.}
$$

The parameter $F$ here is the squared upstream [Froude number](../../../../../froude-number.md). For nonzero discharge, regarding $D$ as a function of $h$, its [derivative](../../../../../derivative.md) is $dD/dh=-1+Q^2/(gh^3)$. It has its unique maximum at $h_c=(Q^2/g)^{1/3}=h_1F^{1/3}$, where the local [Froude number](../../../../../froude-number.md) is one. Substitution gives $D^*=h_1(1-3F^{1/3}/2+F/2)$. This maximum is the [hydraulic control over a smooth hump](../../../../../hydraulic-control-over-a-smooth-hump.md).

## ↑ Ancestors (10)

1. [17D](../17d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

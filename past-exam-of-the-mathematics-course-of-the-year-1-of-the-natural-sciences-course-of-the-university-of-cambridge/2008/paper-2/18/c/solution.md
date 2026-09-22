<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The identity $\nabla\cdot(\boldsymbol a\times\boldsymbol v)=\boldsymbol v\cdot(\nabla\times\boldsymbol a)-\boldsymbol a\cdot(\nabla\times\boldsymbol v)$ reduces to $-\boldsymbol a\cdot(\nabla\times\boldsymbol v)$ when $\boldsymbol a$ is constant. In components, this follows by differentiating $\varepsilon_{ijk}a_jv_k$ and using the antisymmetry of the [Levi-Civita symbol](../../../../../levi-civita-symbol.md). The [divergence theorem](../../../../../divergence-theorem.md) and the cyclic [scalar triple product](../../../../../scalar-triple-product.md) identity now give

$$
\boldsymbol a\cdot\int_S\boldsymbol v\times d\boldsymbol S
=\int_S(\boldsymbol a\times\boldsymbol v)\cdot d\boldsymbol S
=-\boldsymbol a\cdot\int_V\nabla\times\boldsymbol v\,dV.
$$

Since $\boldsymbol a$ is arbitrary,

$$
\boxed{\int_S\boldsymbol v\times d\boldsymbol S=-\int_V\nabla\times\boldsymbol v\,dV.}
$$

The order of the [cross product](../../../../../cross-product.md) determines the minus sign, as in the [vector curl form of the divergence theorem](../../../../../vector-curl-form-of-the-divergence-theorem.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use [Einstein summation convention](../../../../../einstein-notation.md) and write $\partial_j=\nabla_j$. Since $\partial_jr_i=\delta_{ij}$, where $\delta_{ij}$ is the [Kronecker delta](../../../../../kronecker-delta.md), the [product rule](../../../../../product-rule.md) gives

$$
\partial_j(r_iw_j)=\delta_{ij}w_j+r_i\partial_jw_j=w_i+P_i.
$$

This proves $\boxed{P_i=\partial_j(r_iw_j)-w_i}$. Now take $w_j=\partial_j\psi$. Integrating this identity and applying the [divergence theorem](../../../../../divergence-theorem.md) to the first term gives

$$
\int_Vr_i\nabla^2\psi\,dV=\int_Sr_i\partial_j\psi\,dS_j-\int_V\partial_i\psi\,dV.
$$

Part (b) changes the last [volume integral](../../../../../volume-integral.md) of the [gradient](../../../../../gradient.md) into a [surface integral](../../../../../surface-integral.md), yielding

$$
\boxed{\int_Vr_i\nabla^2\psi\,dV=\int_Sr_i\partial_j\psi\,dS_j-\int_S\psi\,dS_i.}
$$

Here $dS_i=\hat n_i\,dS$; the [Laplacian](../../../../../laplacian.md) is $\nabla^2\psi=\partial_j\partial_j\psi$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

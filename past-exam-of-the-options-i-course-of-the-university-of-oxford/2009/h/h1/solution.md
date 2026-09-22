<h1 id="h/h1/solution">Solution</h1>

↑ **Parent:** [H1](../h1.md)

With $\mathbf d=\mathbf q_1-\mathbf q_2$ and $r=|\mathbf d|$, the [Lagrangian](../../../../lagrangian.md) is

$$
L=\frac12\sum_{j=1}^3m_j|\dot{\mathbf q}_j|^2-f(r).
$$

At configurations with $r>0$, the [Euler-Lagrange equations](../../../../euler-lagrange-equation.md) give

$$
m_1\ddot{\mathbf q}_1=-\frac{f'(r)}r\mathbf d,\qquad
m_2\ddot{\mathbf q}_2=\frac{f'(r)}r\mathbf d,\qquad
m_3\ddot{\mathbf q}_3=0.
$$

These formulas apply on the differentiable part of the potential; collision configurations require any additional smooth extension of $f(|\mathbf d|)$ to be specified. Summing the equations gives

$$
\frac d{dt}\sum_jm_j\dot{\mathbf q}_j=0,
$$

so the total [linear momentum](../../../../momentum-split.md) is conserved. The total [energy](../../../../energy-split.md) is

$$
E=\frac12\sum_jm_j|\dot{\mathbf q}_j|^2+f(r).
$$

Differentiating, the two interacting forces do work $-f'(r)\dot r$, while the potential derivative is $f'(r)\dot r$ and particle three contributes no force term. Hence $\dot E=0$. Both **total momentum and total [energy](../../../../energy-split.md) are conserved**.

## ↑ Ancestors (12)

1. [H1](../h1.md)
2. [H](../../h.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

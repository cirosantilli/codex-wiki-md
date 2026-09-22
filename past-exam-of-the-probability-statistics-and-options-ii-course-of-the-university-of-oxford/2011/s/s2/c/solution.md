<h1 id="s/s2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\phi$ denote the standard normal density. Under the shifted sampling density $q(y)=\phi(y-c)$, the [likelihood ratio](../../../../../likelihood-ratio.md) is $\phi(y)/q(y)=e^{-cy+c^2/2}$. Simulate independent $Y_k\sim N(c,1)$ and use

$$
\boxed{\widehat z_c=\frac1n\sum_{k=1}^n\mathbf1_{\{Y_k>c\}}e^{-cY_k+c^2/2}.}
$$

Multiplying the weight by $q$ restores the original density, so each summand $H$ has [expectation](../../../../../expected-value-split.md) $\int_c^\infty\phi(y)\,dy=z_c$. The estimator is unbiased. For the second moment,

$$
\mathbb E_qH^2=\int_c^\infty e^{-cy+c^2/2}\phi(y)\,dy
\leq e^{-c^2/2}z_c,
$$

because $y\geq c$. Since $nv_c=\mathbb E_qH^2-z_c^2$,

$$
\boxed{nv_c+z_c^2\leq e^{-c^2/2}z_c.}
$$

For $c>0$, $e^{-c^2/2}<1$ and $z_c>0$, so $nv_c<z_c-z_c^2=nv_0$, proving $v_c<v_0$. Nonnegativity of [variance](../../../../../variance-split.md) also implies $z_c^2\leq e^{-c^2/2}z_c$; division by the positive $z_c$ gives

$$
\boxed{z_c\leq e^{-c^2/2}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

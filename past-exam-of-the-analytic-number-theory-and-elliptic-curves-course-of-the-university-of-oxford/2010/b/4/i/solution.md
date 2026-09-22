<h1 id="b/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $d=|f'(a_0)|>0$ and $q_0=|f(a_0)|/d^2<1$. At any step before reaching a root, set

$$
a_{i+1}=a_i+h_i,\qquad h_i=-\frac{f(a_i)}{f'(a_i)}.
$$

Assuming inductively that $|f'(a_i)|=d$ and $q_i=|f(a_i)|/d^2<1$, this gives

$$
\boxed{|a_{i+1}-a_i|=\frac{|f(a_i)|}{|f'(a_i)|}=dq_i.}
$$

All derivatives of a [polynomial](../../../../../polynomial-split.md) over $R$ are integral on $R$, so $d\le1$. Hence $|h_i|<1$, and the [ultrametric inequality](../../../../../ultrametric-inequality.md) keeps $a_{i+1}$ in $R$. If a root is reached, retain that value for subsequent terms, and the asserted weak step inequality still holds.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

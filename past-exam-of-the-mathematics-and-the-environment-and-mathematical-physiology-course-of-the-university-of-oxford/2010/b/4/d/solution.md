<h1 id="b/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an [outer solution](../../../../../outer-expansion.md) with bounded derivatives as $\epsilon\to0$, the final complex equation gives $r_n=0$. Working backwards in $0=r_i-r_{i+1}$ then gives every $r_i=0$, including $r_1$; setting only their sum to zero would not suffice. This is the [quasi-steady-state approximation](../../../../../quasi-steady-state-approximation.md), valid after the initial complex-formation layer with the relevant dimensionless rate parameters held fixed.

The recurrence is $C_i=SC_{i-1}/K_i$, where $K_i=(k_{-i}+k_i^+)/k_i$. Thus $C_j=\phi_jS^jC_0$, $\phi_j=\prod_{i=1}^jK_i^{-1}$. Substitution into [enzyme conservation](../../../../../enzyme-conservation.md) yields

$$
C_0=\frac{E_0}{1+\sum_{j=1}^n\phi_jS^j},\qquad C_j=\frac{E_0\phi_jS^j}{1+\sum_{\ell=1}^n\phi_\ell S^\ell}.
$$

Each state $j$ produces [reaction product](../../../../../product-chemistry.md) at rate $k_j^+C_j$, so

$$
\boxed{\rho=E_0\frac{\sum_{j=1}^nk_j^+\phi_jS^j}{1+\sum_{j=1}^n\phi_jS^j}.}
$$

The source's uppercase $N$ in the index range is read as the number $n$ of binding sites. This approximation preserves the total [enzyme](../../../../../enzyme-split.md) population and the different catalytic rates of the occupied states.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

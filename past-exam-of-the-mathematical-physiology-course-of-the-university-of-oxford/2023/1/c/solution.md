<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Normalize the total channel density to one. For [independent permissive gates in an ion channel](../../../../independent-permissive-gates-in-an-ion-channel.md), the [probability](../../../../probability.md) that the $M$ gate is open is $m$, and the [probability](../../../../probability.md) that the $H$ gate is open is $h$. The joint [probability](../../../../probability.md) is the product of the appropriate open or closed [probabilities](../../../../probability.md), giving

$$
\boxed{S_{ij}=m^i(1-m)^{1-i}h^j(1-h)^{1-j}.}
$$

In particular

$$
S_{00}=(1-m)(1-h),\quad S_{10}=m(1-h),\quad
S_{01}=(1-m)h,\quad S_{11}=mh.
$$

The original PDF really prints $j$, rather than $1-j$, on the final factor. That expression fails [normalization of a probability distribution](../../../../normalization-of-a-probability-distribution.md) and does not give the closed-$H$ [probability](../../../../probability.md) at $j=0$; the displayed correction is necessary. If $S_{ij}$ are literal densities with conserved total density $N$, multiply each expression by $N$.

The product additionally assumes initially [independent events](../../../../independent-events.md) and independent gate transitions. The transition scheme alone permits initially correlated gates and does not force this factorization at every time. The all-closed initial preparation used below satisfies the required product assumption.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

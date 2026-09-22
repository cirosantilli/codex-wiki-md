<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the [weakly convergent](../../../../../weak-convergence.md) [subsequence](../../../../../subsequence.md) in (i), with limit $u\in H_0^1(B)$. For each $\phi\in H_0^1(B)$, the [weak formulation](../../../../../weak-formulation.md) gives

$$
\int_B\nabla u_{m_j}\cdot\nabla\phi\,dx=\int_Bf_{m_j}\phi\,dx.
$$

The left side tends to $\int\nabla u\cdot\nabla\phi$ by [weak convergence](../../../../../weak-convergence.md) in $H^1$. The zero-boundary [Sobolev inequality](../../../../../sobolev-inequality.md) gives $\phi\in L^6(B)$, so (ii) makes the right side tend to zero. Taking $\phi=u$ in the limiting identity yields $\int_B|\nabla u|^2=0$. The zero-boundary [Poincaré inequality](../../../../../poincare-inequality.md) then gives $u=0$.

The same argument applies to a [weakly convergent](../../../../../weak-convergence.md) [subsequence](../../../../../subsequence.md) of any [subsequence](../../../../../subsequence.md) of $(u_m)$, because all remain bounded as in (i). To see why this proves convergence of the full sequence, suppose a continuous [linear functional](../../../../../linear-functional.md) $F$ on $H^1(B)$ did not satisfy $F(u_m)\to0$. Some [subsequence](../../../../../subsequence.md) would have $|F(u_{m_j})|\geq\varepsilon>0$. Its boundedness gives a further [weakly convergent](../../../../../weak-convergence.md) [subsequence](../../../../../subsequence.md), whose limit has just been proved to be zero; then $F$ tends to zero along it, a contradiction. Therefore

$$
\boxed{u_m\rightharpoonup0\quad\text{in }H^1(B)\text{ for the entire sequence}.}
$$

Uniqueness of a possible limit alone is not enough without the [weak sequential compactness in a Hilbert space](../../../../../weak-sequential-compactness-in-a-hilbert-space.md) used to extract a further [subsequence](../../../../../subsequence.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

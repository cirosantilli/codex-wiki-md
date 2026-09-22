<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each state, add its incoming [reaction rates](../../../../reaction-rate.md) and subtract its outgoing [reaction rates](../../../../reaction-rate.md). This gives the [master equation](../../../../master-equation.md)

$$
\boxed{\begin{aligned}
\dot S_{00}&=-(\alpha+\gamma)S_{00}+\beta S_{10}+\delta S_{01},\\
\dot S_{10}&=\alpha S_{00}-(\beta+\gamma)S_{10}+\delta S_{11},\\
\dot S_{01}&=\gamma S_{00}-(\alpha+\delta)S_{01}+\beta S_{11},\\
\dot S_{11}&=\gamma S_{10}+\alpha S_{01}-(\beta+\delta)S_{11}.
\end{aligned}}
$$

Summing gives $\sum_{i,j}\dot S_{ij}=0$, verifying the [conservation law](../../../../conservation-law.md) for total channel density. Nonnegative initial densities stay nonnegative because every loss term vanishes when its own density reaches zero.

## ↑ Ancestors (12)

1. [D](../d.md)
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

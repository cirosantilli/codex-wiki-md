<h1 id="2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use reversible [quantum arithmetic](../../../../../../../quantum-arithmetic.md) on an ancillary work register. On each computational-basis branch, compute

$$
|i\rangle|0\rangle|0\rangle
\longmapsto
|i\rangle|A_i\rangle|B_i\rangle
\longmapsto
|i\rangle|A_i\rangle|B_i\rangle|\theta_i\rangle,
$$

where

$$
f_i=\frac{A_i}{B_i},
\qquad
\theta_i=\arccos\sqrt{f_i}.
$$

Because the classical algorithms for $A_i$ and $B_i$ are efficient, they can be made reversible with polynomial overhead. Reversible division, square root, and inverse cosine to the retained binary precision likewise use $\operatorname{poly}(\log N)$ gates under the question's precision convention. Uncompute the $A_i$ and $B_i$ work registers, leaving

$$
\boxed{
|\widetilde\psi_m\rangle
=\sum_{i=0}^{2^m-1}\sqrt{p_i^{(m)}}|i\rangle|\theta_i\rangle}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

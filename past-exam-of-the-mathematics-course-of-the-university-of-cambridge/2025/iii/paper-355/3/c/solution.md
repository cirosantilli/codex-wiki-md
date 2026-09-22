<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the pair energy as

$$
U_{A_H}(\Gamma)=U_{\rm rep}(\Gamma)-A_HW(\Gamma),
\qquad W(\Gamma)>0.
$$

At $A_H=0$ the interaction is repulsive, so the Mayer integrand and hence $B_2$ are positive. Increasing $A_H$ strengthens attraction and

$$
\frac{dB_2}{dA_H}
=-\frac1{2k_BT}\int
W(\Gamma)e^{-U_{A_H}(\Gamma)/(k_BT)}\,d\Gamma<0.
$$

For sufficiently strong attraction, negative configurations dominate and $B_2<0$. Continuity therefore gives a critical $A_H^*$ with $B_2(A_H^*)=0$. The [Taylor theorem](../../../../../../taylor-theorem.md) gives

$$
\boxed{
B_2(A_H)
=B_2'(A_H^*)(A_H-A_H^*)+\cdots
\sim r(A_H^*-A_H)},
$$

where $r=-B_2'(A_H^*)>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 355](../../../paper-355-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

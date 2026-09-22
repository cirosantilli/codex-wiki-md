<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose nonzero vectors $p_i\in\mathbb F^2$ representing $P_i$, and write $[u,v]=\det(u,v)$. Use the [cross-ratio](../../../../../cross-ratio.md) convention

$$
\boxed{(P_0P_1:P_2P_3)=\frac{[p_0,p_2][p_1,p_3]}{[p_0,p_3][p_1,p_2]}.}
$$

Distinctness makes the denominator nonzero. Every rescaling of a representative occurs once in numerator and denominator, so the value depends only on the [projective points](../../../../../projective-point.md). Swapping both pairs simply exchanges the numerator's factors and the denominator's factors:

$$
(P_1P_0:P_3P_2)=\frac{[p_1,p_3][p_0,p_2]}{[p_1,p_2][p_0,p_3]}=(P_0P_1:P_2P_3).
$$

Under an invertible [linear map](../../../../../linear-map.md) $A$, $[Au,Av]=\det(A)[u,v]$. Two factors of $\det(A)$ occur above and below the fraction, proving [projective transformation](../../../../../projective-linear-transformation.md) invariance.

Finally choose [homogeneous coordinates](../../../../../homogeneous-coordinate.md) making $P_0=[1:0]$, $P_1=[0:1]$, $P_2=[1:1]$. This normalization exists by the allowed theorem about a [projective frame](../../../../../projective-frame.md). A point distinct from $P_0$ is uniquely $[t:1]$, and the displayed [cross-ratio](../../../../../cross-ratio.md) is $t$. Thus equality of the two [cross-ratios](../../../../../cross-ratio.md) forces equal coordinates and

$$
\boxed{P_3=Q.}
$$

This also shows that for fixed first three distinct points the fourth point is determined by its [cross-ratio](../../../../../cross-ratio.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

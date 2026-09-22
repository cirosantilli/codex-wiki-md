<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Apply the first extraction move to the two outer occurrences of $x$, then cyclically rotate the word to expose the two occurrences of $y^{-1}$:

$$
\begin{aligned}
xyzzyx
&\sim xx\,y^{-1}z^{-1}z^{-1}y^{-1}\\
&\sim y^{-1}z^{-1}z^{-1}y^{-1}xx\\
&\sim y^{-1}y^{-1}zzxx\\
&\sim xx\,y^{-1}y^{-1}zz.
\end{aligned}
$$

In the third line the repeated letter for the move is $y^{-1}$, and the intervening string is $z^{-1}z^{-1}$, whose inverse is $zz$. Rename $y^{-1}$ as a new edge label. The final word has the standard form $aabbcc$.

Each same-direction repeated pair represents a projective-plane summand, so the [classification theorem for surfaces](../../../../../classification-theorem-for-surfaces.md) identifies this word with the [connected sum](../../../../../connected-sum-of-oriented-manifolds.md) of three real projective planes:

$$
\boxed{S\cong\mathbb{RP}^2\mathbin{\#}\mathbb{RP}^2\mathbin{\#}\mathbb{RP}^2.}
$$

Thus the surface has [crosscap number](../../../../../crosscap-number.md) three. As a check, the original identifications make all six polygon vertices equivalent, leaving one [vertex](../../../../../vertex-graph-theory.md), three edges and one face. Its [Euler characteristic](../../../../../euler-characteristic.md) is $1-3+1=-1=2-3$, consistent with that crosscap count.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

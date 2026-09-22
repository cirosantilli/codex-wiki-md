<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $I=(X^3)_T$ and $J=(Y^3)_{\mathbb R[Y]}$. Part (b)(i) gives a unique representative $a+bX^2+cX^4$ for each element of the [quotient ring](../../../../../quotient-ring.md) $T/I$. By [polynomial division](../../../../../polynomial-division.md), each element of the [quotient ring](../../../../../quotient-ring.md) $\mathbb R[Y]/J$ likewise has a unique representative $a+bY+cY^2$. Thus the proposed map $\Phi$ is well-defined and a [bijection](../../../../../bijection.md).

It preserves [addition](../../../../../addition.md) and $1$. To verify [multiplication](../../../../../multiplication.md), all terms of [polynomial degree](../../../../../degree-of-a-polynomial.md) at least $5$ lie in $I$. Hence

$$
\begin{aligned}
&(a+bX^2+cX^4)(a'+b'X^2+c'X^4)+I\\
&\qquad=aa'+(ab'+ba')X^2+(ac'+bb'+ca')X^4+I.
\end{aligned}
$$

In the other [quotient ring](../../../../../quotient-ring.md), $Y^3=0$, giving exactly the same [coefficient](../../../../../coefficient.md) formula:

$$
(a+bY+cY^2)(a'+b'Y+c'Y^2)+J
=aa'+(ab'+ba')Y+(ac'+bb'+ca')Y^2+J.
$$

Therefore

$$
\boxed{\Phi:T/(X^3)_T\xrightarrow{\ \cong\ }\mathbb R[Y]/(Y^3),\qquad
a+bX^2+cX^4+I\longmapsto a+bY+cY^2+J}
$$

is a [ring isomorphism](../../../../../ring-isomorphism.md). Both sides are examples of a [truncated polynomial ring](../../../../../truncated-polynomial-ring.md); the generator on the left is the class of $X^2$, whose square is nonzero and whose cube vanishes.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

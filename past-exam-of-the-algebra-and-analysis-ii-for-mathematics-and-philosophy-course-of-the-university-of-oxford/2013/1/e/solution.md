<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Part (b) requires $m_T$ to be a monic [divisor](../../../../divisor.md) of $x^2(x-1)$. The constant [divisor](../../../../divisor.md) one cannot annihilate a nonzero [vector space](../../../../vector-space-split.md). Every remaining [divisor](../../../../divisor.md) can occur in dimension three:

$$
\boxed{m_T\in\{x,\ x^2,\ x-1,\ x(x-1),\ x^2(x-1)\}.}
$$

Here are corresponding [matrices](../../../../matrix.md), all satisfying $T^3-T^2=0$:

$$
\begin{array}{c|c}
m_T&\text{matrix of }T\\\hline
x&0_{3\times3}\\
x^2&\begin{pmatrix}0&1&0\\0&0&0\\0&0&0\end{pmatrix}\\
x-1&I_3\\
x(x-1)&\operatorname{diag}(0,0,1)\\
x^2(x-1)&\begin{pmatrix}0&1&0\\0&0&0\\0&0&1\end{pmatrix}
\end{array}
$$

The last [matrix](../../../../matrix.md) contains a size-two [nilpotent](../../../../nilpotent.md) [Jordan block](../../../../jordan-block.md), requiring the factor $x^2$, and an [eigenvector](../../../../eigenvector.md) with [eigenvalue](../../../../eigenvalue.md) one, requiring $x-1$. Thus its [minimal polynomial](../../../../minimal-polynomial.md) is exactly $f$. The [zero matrix](../../../../zero-matrix.md) has [minimal polynomial](../../../../minimal-polynomial.md) $x\neq f$, providing the other requested example.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Algebra and analysis II for mathematics and philosophy course of the University of Oxford](../../../../algebra-and-analysis-ii-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Direct [matrix multiplication](../../../../matrix-multiplication.md) gives $A^2=0$. Denote the columns by $c_1,\ldots,c_4$; they satisfy

$$
c_3=c_1-2c_2,\qquad c_4=-c_1+c_2.
$$

Thus the [matrix rank](../../../../matrix-rank.md) is at most two. Over the [real numbers](../../../../real-number.md) or [complex numbers](../../../../complex-number.md), the upper-left two-by-two [minor](../../../../minor-linear-algebra.md) is $-3\ne0$, so the [matrix rank](../../../../matrix-rank.md) is exactly two. Every [Jordan block](../../../../jordan-block.md) has size at most two because $A^2=0$, and each size-two [Nilpotent Jordan block](../../../../nilpotent-jordan-block.md) contributes one to the [matrix rank](../../../../matrix-rank.md). Consequently

$$
\boxed{J=J_2(0)\oplus J_2(0)=
\begin{pmatrix}0&1&0&0\\0&0&0&0\\0&0&0&1\\0&0&0&0\end{pmatrix}}.
$$

Equivalently the [nullities](../../../../nullity-of-a-linear-map.md) are $(2,4)$ and the [minimal polynomial](../../../../minimal-polynomial.md) is $x^2$.

There is a [field](../../../../field.md) qualification in the source: Question 2 initially allows an arbitrary [field](../../../../field.md), and part (c) does not specify a new one. The preceding answer holds over every [field](../../../../field.md) whose [characteristic](../../../../characteristic-of-a-field.md) is not three. In [characteristic](../../../../characteristic-of-a-field.md) three, the first row vanishes and the other three rows all become $(2,1,0,2)$, giving [matrix rank](../../../../matrix-rank.md) one while $A^2=0$. Under that reading the answer is instead

$$
\boxed{J=J_2(0)\oplus J_1(0)\oplus J_1(0)\qquad(\operatorname{char}F=3)}.
$$

## ↑ Ancestors (12)

1. [c](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

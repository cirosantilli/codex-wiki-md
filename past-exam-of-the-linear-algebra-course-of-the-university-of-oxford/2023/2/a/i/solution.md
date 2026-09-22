<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Write $K_i=\ker T^i$, with $K_0=\{0\}$. The [minimal polynomial](../../../../../minimal-polynomial.md) $x^m$ means $T^m=0$ and $T^{m-1}\ne0$. Choose $w$ with $T^{m-1}w\ne0$. For each $0\leq i<m$, set $w_i=T^{m-1-i}w$. Then

$$
T^{i+1}w_i=0,\qquad T^iw_i=T^{m-1}w\ne0.
$$

Thus $w_i\in K_{i+1}\setminus K_i$. Also $K_i\subseteq K_{i+1}$ because applying $T$ to zero still gives zero. Therefore the [kernel dimensions of powers of a nilpotent map](../../../../../kernel-dimensions-of-powers-of-a-nilpotent-map.md) increase strictly until the [nilpotency index](../../../../../nilpotency-index.md):

$$
\boxed{\{0\}=K_0\subsetneq K_1\subsetneq\cdots\subsetneq K_m=V}.
$$

The same reasoning covers $m=1$, when the [nilpotent linear map](../../../../../nilpotent-linear-map.md) is zero on a nonzero [vector space](../../../../../vector-space-split.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

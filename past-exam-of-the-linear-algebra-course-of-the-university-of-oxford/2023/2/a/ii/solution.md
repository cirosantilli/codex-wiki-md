<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Put $d_i=\dim K_i$, including $d_0=0$. The [restriction](../../../../../restriction-mathematics.md) of $T^i$ to $K_{i+1}$ has [kernel](../../../../../kernel-of-a-linear-map-split.md) $K_i$, so the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives

$$
\dim T^i(K_{i+1})=d_{i+1}-d_i.
$$

Likewise $T^{i-1}|_{K_i}$ has [kernel](../../../../../kernel-of-a-linear-map-split.md) $K_{i-1}$ and hence image [dimension](../../../../../dimension-vector-space.md) $d_i-d_{i-1}$. But $T(K_{i+1})\subseteq K_i$, which implies

$$
T^i(K_{i+1})=T^{i-1}(T(K_{i+1}))\subseteq T^{i-1}(K_i).
$$

Comparing [dimensions](../../../../../dimension-vector-space.md) yields the required concavity of the [kernel dimensions of powers of a nilpotent map](../../../../../kernel-dimensions-of-powers-of-a-nilpotent-map.md):

$$
\boxed{d_{i+1}-d_i\leq d_i-d_{i-1},\qquad 2d_i\geq d_{i-1}+d_{i+1}\quad(1\leq i<m)}.
$$

## ↑ Ancestors (13)

1. [ii](../ii.md)
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

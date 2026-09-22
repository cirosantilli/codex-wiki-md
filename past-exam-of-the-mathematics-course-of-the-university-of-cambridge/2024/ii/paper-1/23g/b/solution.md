<h1 id="23g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $f_z(y)=f(yz)$, the substitution $u=yz$ gives

$$
\|f_z\|_p^p=z^{-1}\|f\|_p^p,
\qquad
\|f_z\|_p=z^{-1/p}\|f\|_p.
$$

Homogeneity of $K$ and the substitution $x=yz$ give

$$
Tf(y)=\int_0^\infty K(yz,y)f(yz)y\,dz
     =\int_0^\infty K(z,1)f_z(y)\,dz.
$$

Apply part (a), or equivalently the [Minkowski integral inequality](../../../../../../minkowski-integral-inequality.md), to this [integral](../../../../../../integral.md) and use the preceding scaling identity:

$$
\begin{aligned}
\|Tf\|_p
&\leq\int_0^\infty |K(z,1)|\,\|f_z\|_p\,dz\\
&=\|f\|_p\int_0^\infty |K(z,1)|z^{-1/p}\,dz\\
&=\|f\|_p.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23G](../../23g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

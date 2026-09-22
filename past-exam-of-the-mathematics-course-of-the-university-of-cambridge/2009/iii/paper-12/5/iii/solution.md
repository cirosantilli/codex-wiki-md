<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $m=\inf_{\mathbb R^n}u$, which is finite because $u$ is bounded, and put $v=u-m$. Then $v\geq0$ is harmonic. Choose points $y_j$ with $v(y_j)\to0$. For any fixed $x$, choose $r_j$ large enough that $x,y_j\in B_{r_j}(0)$. Since $v$ is harmonic on all of $\mathbb R^n$, the [Harnack inequality for harmonic functions](../../../../../../harnack-inequality-for-harmonic-functions.md) on $B_{4r_j}(0)$ gives

$$
0\leq v(x)\leq3^nv(y_j)\longrightarrow0.
$$

The comparison factor is independent of the growing radius, which is essential. Thus $v(x)=0$ for every $x$ and

$$
\boxed{u\equiv m\text{ on }\mathbb R^n.}
$$

This proves the [Liouville theorem for harmonic functions](../../../../../../harmonic-liouville-theorem.md) in every dimension. In fact the argument only needs an entire harmonic function to be bounded below; changing its sign gives the corresponding bounded-above result.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

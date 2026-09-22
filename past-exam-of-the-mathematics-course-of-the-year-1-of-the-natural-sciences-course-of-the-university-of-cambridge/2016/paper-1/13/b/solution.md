<h1 id="13/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $L=5\pi/2$. The curve tangent is $\mathbf r'=(-b\sin\theta,b\cos\theta,c)$. For the first [line integral](../../../../../line-integral.md), the [scalar triple product](../../../../../scalar-triple-product.md) identity gives $(\mathbf a\times\mathbf r)\cdot\mathbf r'=\mathbf a\cdot(\mathbf r\times\mathbf r')$. Its [cross product](../../../../../cross-product.md) is

$$
\mathbf r\times\mathbf r'=\bigl(bc(\sin\theta-\theta\cos\theta),\ -bc(\theta\sin\theta+\cos\theta),\ b^2\bigr).
$$

The needed [definite integrals](../../../../../definite-integral.md) are

$$
\int_0^L(\sin\theta-\theta\cos\theta)d\theta
=\big[-\theta\sin\theta-2\cos\theta\big]_0^L=2-L,
$$

and $\int_0^L(-\theta\sin\theta-\cos\theta)d\theta=[\theta\cos\theta-2\sin\theta]_0^L=-2$. Hence

$$
\boxed{I_1=bc\left(2-\frac{5\pi}{2}\right)a_x-2bc\,a_y+\frac{5\pi b^2}{2}a_z.}
$$

For the second [line integral](../../../../../line-integral.md), substitute the curve into $\mathbf v_2\cdot\mathbf r'$. The cubic terms combine to $b^3\cos\theta$, leaving

$$
\begin{aligned}
\mathbf v_2\cdot\mathbf r'
&=b^3\cos\theta+bc^2\theta^2\cos\theta+2bc^2\theta\sin\theta\\
&=\frac d{d\theta}\left[b\sin\theta\,(b^2+c^2\theta^2)\right].
\end{aligned}
$$

The [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) therefore gives

$$
\boxed{I_2=b\left(b^2+\frac{25\pi^2c^2}{4}\right).}
$$

Both calculations retain the full path from $\theta=0$ to $5\pi/2$, rather than inadvertently closing the [helix](../../../../../helix.md) after one turn.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [13](../../13.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

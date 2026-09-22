<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x=0,1,2$, the value of $x^3-x-1$ is the nonsquare $2$ in $\mathbb F_3$. Thus the point at infinity is the only rational point and

$$
\#E(\mathbb F_3)=1,
\qquad a_3=3+1-1=3.
$$

The eigenvalues of the [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) are the roots

$$
\alpha,\beta=\frac{3\pm i\sqrt3}{2}=\sqrt3e^{\pm i\pi/6}
$$

of $T^2-3T+3$. The [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) gives

$$
\#E(\mathbb F_{3^r})=3^r+1-\alpha^r-\beta^r
=3^r+1-2\cdot3^{r/2}\cos(r\pi/6).
$$

The last term vanishes exactly when $r\pi/6\equiv\pi/2\pmod\pi$. Hence

$$
\boxed{\#E(\mathbb F_{3^r})=3^r+1\quad\Longleftrightarrow\quad r\equiv3\pmod6.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

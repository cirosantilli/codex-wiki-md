<h1 id="22h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The real [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) states that for every bounded linear functional $f:H\to\mathbb R$ on a real Hilbert space there is a unique $y\in H$ such that

$$
f(x)=\langle x,y\rangle
\qquad(x\in H),
$$

and $\|f\|=\|y\|$.

If $f=0$, take $y=0$. Otherwise $Y=\ker f$ is a closed proper subspace, so the supplied [orthogonal decomposition by a closed subspace](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) gives a nonzero $z\in Y^\perp$. Since $f(z)\ne0$, for every $x\in H$,

$$
x-\frac{f(x)}{f(z)}z\in Y.
$$

Taking its inner product with $z$ yields

$$
\langle x,z\rangle
=\frac{f(x)}{f(z)}\|z\|^2,
$$

and therefore

$$
f(x)=\left\langle x,\frac{f(z)}{\|z\|^2}z\right\rangle.
$$

Thus $y=f(z)z/\|z\|^2$ represents $f$. If both $y$ and $y'$ represent it, then $\langle x,y-y'\rangle=0$ for every $x$; taking $x=y-y'$ proves uniqueness. Finally, [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $\|f\|\leq\|y\|$, while evaluating at $x=y/\|y\|$ when $y\ne0$ gives the reverse inequality. Hence

$$
\boxed{f(x)=\langle x,y\rangle,
\qquad\|f\|=\|y\|.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22H](../../22h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

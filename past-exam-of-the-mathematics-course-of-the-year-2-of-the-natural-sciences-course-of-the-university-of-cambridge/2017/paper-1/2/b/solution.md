<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The transformed endpoint values are $u(0,t)=0$ and $u(\pi,t)=3$. Apply [boundary lifting](../../../../../boundary-lifting.md) with $u=3x/\pi+w$. The lifted profile is linear, so $w_t=w_{xx}$ with homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) and

$$
w(x,0)=\frac{\sin2x}{\pi}.
$$

For [separation of variables](../../../../../separation-of-variables.md), put $w=X(x)T(t)$. Then $X''/X=T'/T=-\lambda$. The endpoint conditions give nonzero spatial modes only for $\lambda=n^2$, $n=1,2,\ldots$, with $X_n=\sin nx$ and $T_n=e^{-n^2t}$. Hence

$$
w(x,t)=\sum_{n=1}^{\infty}b_ne^{-n^2t}\sin nx,\qquad
b_n=\frac2\pi\int_0^\pi\frac{\sin2x}{\pi}\sin nx\,dx=\frac{\delta_{n2}}\pi,
$$

by [orthogonality](../../../../../orthogonal-vectors.md) of the sine modes. Only the $n=2$ mode is present. Undoing both substitutions gives

$$
\boxed{v(x,t)=\frac{(t+1)^2}{\pi}\left(3x+e^{-4t}\sin2x\right).}
$$

At $t=0$ this has the prescribed initial profile, and at $x=\pi$ it is $3(t+1)^2$. Differentiating also verifies the original evolution equation directly.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

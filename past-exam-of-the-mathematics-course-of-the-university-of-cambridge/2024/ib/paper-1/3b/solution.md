<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Since

$$
f'(z)=\pi\sinh(\pi z),
$$

the critical points are exactly

$$
\boxed{z=ki\quad(k\in\mathbb Z)}.
$$

The [holomorphic inverse function theorem](../../../../../holomorphic-inverse-function-theorem.md) shows that $f$ is conformal locally everywhere else.

For $z=x+iy$,

$$
f(z)=\cosh(\pi x)\cos(\pi y)
+i\sinh(\pi x)\sin(\pi y).
$$

Its imaginary part is positive throughout $S$. On the three boundary pieces,

$$
\begin{aligned}
L_1&:\quad f(x)=\cosh(\pi x)\in(1,\infty),\\
L_2&:\quad f(iy)=\cos(\pi y)\in(-1,1),\\
L_3&:\quad f(x+i)=-\cosh(\pi x)\in(-\infty,-1).
\end{aligned}
$$

These intervals traverse the boundary of the upper half-plane. The inverse branch

$$
z=\frac1\pi\operatorname{arcosh}\zeta,
\qquad \Re z>0,\quad0<\Im z<1,
$$

exists for $\Im\zeta>0$, proving that the image is precisely

$$
\boxed{f(S)=\{\zeta:\Im\zeta>0\}}.
$$

This is the [hyperbolic-cosine half-strip map](../../../../../hyperbolic-cosine-half-strip-map.md).

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

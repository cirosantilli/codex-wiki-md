<h1 id="analysis/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Laurent's theorem](../../../../laurent-theorem.md) states that a [holomorphic function](../../../../holomorphic-function-split.md) on $R<|z-a|<S$ has a unique expansion $\sum_{n\in\mathbb Z}a_n(z-a)^n$, converging absolutely there and uniformly on [compact](../../../../compact-space.md) subannuli, with

$$
a_n=\frac1{2\pi i}\int_{|z-a|=r}\frac{f(z)}{(z-a)^{n+1}}dz\quad(R<r<S).
$$

Here $\sin z=z(1-z^2/6+\cdots)$ has a [simple zero](../../../../simple-zero.md) at zero and no other zero in $|z|<\pi$. Hence $1/\sin z$ has only a [simple pole](../../../../simple-pole.md) there, giving the stated series with no powers below $z^{-1}$. Multiplying by $\sin z$ and comparing the constant, linear and quadratic coefficients yields

$$
\boxed{c_{-1}=1,\qquad c_0=0,\qquad c_1=1/6.}
$$

Use the coefficient integrals on the two circles. The annular region between them contains exactly the [simple poles](../../../../simple-pole.md) $\pi,-\pi$, and the [residue](../../../../residue.md) of $1/\sin z$ at each is $1/\cos(\pm\pi)=-1$. Apply the [residue theorem](../../../../residue-theorem.md) to $1/(z^{n+1}\sin z)$ between the circles:

$$
\boxed{d_n=c_n-\pi^{-n-1}-(-\pi)^{-n-1}\quad(n\ge-1).}
$$

For lower indices, set $c_n=0$ because the inner [Laurent series](../../../../laurent-series.md) has no such terms; the same contour argument then still applies. Since $f$ is odd, its even-index coefficients vanish. A complete explicit list for the requested range is

$$
\boxed{\begin{aligned}
d_1&=\tfrac16-\frac2{\pi^2},&d_0&=0,&d_{-1}&=-1,\\
d_{-2k}&=0\ (k\ge1),&&d_{-(2k+1)}&=-2\pi^{2k}\ (k\ge1).
\end{aligned}}
$$

The subtraction accounts for the two [poles](../../../../pole.md) crossed; using the inner coefficients unchanged outside their [annulus](../../../../annulus-mathematics.md) would miss precisely these terms.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Analysis](../../analysis.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

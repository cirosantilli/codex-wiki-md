<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

Assume the Laplace integrals converge absolutely in a common right half-plane. The [Fubini theorem](../../../../../fubini-s-theorem.md) and the substitution $t=u-v$ on $u\geq v\geq0$ give the [convolution theorem for Laplace transforms](../../../../../convolution-theorem-for-laplace-transforms.md):

$$
\begin{aligned}
\widehat h(p)&=\int_0^\infty\int_0^u e^{-pu}f(u-v)g(v)\,dv\,du\\
&=\int_0^\infty\int_0^\infty e^{-p(t+v)}f(t)g(v)\,dt\,dv
=\boxed{\widehat f(p)\widehat g(p)}.
\end{aligned}
$$

For the specified inverse-square-root function, the supplied identity says $f*f=\pi$ on $t>0$. Consequently $\widehat f(p)^2=\pi/p$. For real $p>0$ the defining integral is positive, fixing the positive square root; analytic continuation into $\operatorname{Re}p>0$ gives

$$
\boxed{\widehat f(p)=\sqrt\pi\,p^{-1/2},}
$$

with the branch positive on the positive real axis. The square identity alone would not select the sign.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

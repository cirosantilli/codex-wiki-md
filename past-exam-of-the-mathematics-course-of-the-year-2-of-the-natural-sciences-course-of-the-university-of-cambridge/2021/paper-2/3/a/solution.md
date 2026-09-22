<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the real decaying Bessel form used here, take $k>0$. The original PDF has $K_m(r)$ as the last factor in its auxiliary differential equation, although both differentiated factors have argument $kr$; that last argument must also be $kr$ for the stated [Modified Bessel differential equation](../../../../../modified-bessel-differential-equation.md).

Put $B(r)=K_m(kr)$. The corrected identity is $B''=-B'/r+(k^2+m^2/r^2)B$. Since the field is radial, the [radial Laplacian](../../../../../radial-laplacian.md) gives

$$
\begin{aligned}
(\Delta-k^2)(r^{-p}B)
&=r^{-p}\left[B''+\frac{2-2p}{r}B'+\left(\frac{p(p-1)}{r^2}-k^2\right)B\right]\\
&=r^{-p}\left[\frac{1-2p}{r}B'+\frac{p(p-1)+m^2}{r^2}B\right].
\end{aligned}
$$

Away from the point source this must vanish. For $k>0$, a constant ratio of $rB'$ to $B$ would make $B$ a pure power, incompatible with the $k^2r^2$ term of its equation. Therefore both displayed coefficients must vanish:

$$
\boxed{p=\frac12,\qquad m^2=\frac14,\quad\text{so }m=\pm\frac12.}
$$

The two orders give the same [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md): $K_{-1/2}(z)=K_{1/2}(z)=\sqrt{\pi/(2z)}e^{-z}$.[§10.39, equation 10.39.2, equality of the two half-integer orders and their elementary form](../../../../../nist-digital-library-of-mathematical-functions.md)

The source describes $k$ merely as real, but the following displayed real square-root formula implicitly needs $k>0$. For the operator with arbitrary real $k$, its decaying fundamental solution instead uses $\kappa=|k|$; $k=0$ is obtained by a limit. The unmodified real $A K_m(kr)$ ansatz is not a real Bessel formula for all negative $k$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

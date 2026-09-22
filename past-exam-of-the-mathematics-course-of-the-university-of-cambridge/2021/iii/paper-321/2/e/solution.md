<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The specific angular momentum of a circular [Keplerian orbit](../../../../../../kepler-orbit.md) is $\sqrt{GM_*r}$. Therefore the disk angular momentum is

$$
J=\int_0^R\sqrt{GM_*r}\,\Sigma\,2\pi r\,dr
=\sqrt{GM_*}\,B,
$$

where

$$
\boxed{B=\int_0^Rr^{1/2}\Sigma\,2\pi r\,dr}.
$$

The absence of an external or inner-boundary torque makes $J$, and hence $B$, constant.

From $\bar\nu=Ar^{9/2}\Sigma^2$,

$$
[A]=L^{3/2}M^{-2}T^{-1},
\qquad
[B]=ML^{1/2}.
$$

The combination $AB^2t$ has dimension $L^{5/2}$. [Dimensional analysis](../../../../../../dimensional-analysis.md) therefore gives

$$
\boxed{R\propto(AB^2t)^{2/5}\propto t^{2/5}}.
$$

For the supplied [similarity solution](../../../../../../similarity-solution.md), put $\tau=t/t_0$ and $u=\sqrt{r/R(t)}$. Then $r=Ru^2$ and $dr=2Ru\,du$. The total mass is

$$
\begin{aligned}
M_D
&=2\pi\int_0^R\Sigma r\,dr\\
&=4\pi\Sigma_0R_0^{3/2}\tau^{-2/5}R^{1/2}
\int_0^1(1-u)^{1/2}\,du\\
&=\frac{8\pi}{3}\Sigma_0R_0^{3/2}
\tau^{-2/5}R^{1/2}.
\end{aligned}
$$

Since $R^{1/2}=R_0^{1/2}\tau^{1/5}$,

$$
\boxed{M_D=\frac{8\pi}{3}\Sigma_0R_0^2
\left(\frac t{t_0}\right)^{-1/5}}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

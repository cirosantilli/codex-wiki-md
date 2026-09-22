<h1 id="13c/solution">Solution</h1>

↑ **Parent:** [13C](../13c.md)

[Fick's first law](../../../../../fick-s-first-law.md) gives the diffusive flux

$$
\boxed{\mathbf J=-D(C)\nabla C}.
$$

Local [conservation](../../../../../conservation-law.md) says $C_t+\nabla\cdot\mathbf J=0$, and therefore

$$
\boxed{C_t=\nabla\cdot(D(C)\nabla C)}.
$$

For $D(C)=kC$, conservation of the deposited amount requires

$$
2\pi\int_0^\infty rC(r,t)\,dr=2\pi M.
$$

The dimensions satisfy $[M]=[C]L^2$ and $[k]=L^2/([C]T)$. Thus $Mkt$ has dimension $L^4$, so the similarity length is $(Mkt)^{1/4}$. Requiring the concentration scale to have dimension $[C]$ gives

$$
\boxed{\alpha=\beta=\frac12,\qquad\gamma=\frac14}.
$$

Hence

$$
C(r,t)=\sqrt{\frac{M}{kt}}\,F(\xi),
\qquad
\xi=\frac{r}{(Mkt)^{1/4}},
\qquad
\int_0^\infty\xi F(\xi)\,d\xi=1.
$$

In polar coordinates, substitution into  
$C_t=k r^{-1}(rCC_r)_r$ gives

$$
-\frac12F-\frac14\xi F'
=\frac1\xi(\xi FF')'.
$$

Multiplying by $\xi$ and integrating once, with regularity and zero radial flux at the origin, yields

$$
\xi FF'=-\frac14\xi^2F.
$$

Where $F>0$, this reduces to $F'=-\xi/4$, so

$$
F(\xi)=A-\frac{\xi^2}{8}.
$$

Nonnegativity and zero flux at the moving front give the compactly supported profile

$$
F(\xi)=\left(A-\frac{\xi^2}{8}\right)_+,
\qquad
\xi_0^2=8A.
$$

The normalization gives

$$
1=\int_0^{\xi_0}\xi\left(A-\frac{\xi^2}{8}\right)d\xi
=2A^2,
$$

and hence $A=1/\sqrt2$ and $\xi_0^4=32$. This is the [Two-dimensional Barenblatt solution with diffusivity proportional to concentration](../../../../../two-dimensional-barenblatt-solution-with-diffusivity-proportional-to-concentration.md), and its support radius is

$$
\boxed{r_0(t)=(32Mkt)^{1/4}},
$$

so $N=32$.

Now add the linear reaction term and write

$$
C(r,t)=e^{at}G(r,\tau(t)).
$$

Substitution cancels the terms $aC$ and leaves

$$
e^{at}\tau'G_\tau
=ke^{2at}\nabla\cdot(G\nabla G).
$$

Choosing

$$
\boxed{\tau'=e^{at},\qquad
\tau(t)=
\begin{cases}
(e^{at}-1)/a,&a\ne0,\\
t,&a=0
\end{cases}}
$$

produces $G_\tau=k\nabla\cdot(G\nabla G)$, as in the [linear-reaction time change for quadratic nonlinear diffusion](../../../../../linear-reaction-time-change-for-quadratic-nonlinear-diffusion.md). Therefore

$$
\boxed{
C(r,t)=e^{at}\sqrt{\frac{M}{k\tau(t)}}
\left(
\frac1{\sqrt2}
-\frac{r^2}{8\sqrt{Mk\tau(t)}}
\right)_+
}.
$$

For $a=0$, the front grows like $t^{1/4}$ while the central concentration decays like $t^{-1/2}$. For $a>0$, $\tau\sim e^{at}/a$, so the front grows like $e^{at/4}$ and the central concentration like $e^{at/2}$. For $a<0$, $\tau\to1/|a|$: the front approaches a finite limiting radius while the concentration decays exponentially to zero.

## ↑ Ancestors (10)

1. [13C](../13c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

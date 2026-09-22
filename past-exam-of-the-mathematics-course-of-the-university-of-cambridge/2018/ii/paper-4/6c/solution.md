<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Let

$$
F(N)=\frac{rN}{(1+bN)^2}.
$$

At low density, $F(N)/N\to r$, so $r$ is the density-independent per-generation multiplication factor. The parameter $b$ has units of inverse population and sets the density scale at which crowding suppresses recruitment.

The [fixed points](../../../../../fixed-point.md) satisfy $N=F(N)$. Besides extinction $N=0$, for $r>1$ there is the positive fixed point

$$
\boxed{N_*=\frac{\sqrt r-1}{b}.}
$$

Since

$$
F'(N)=\frac{r(1-bN)}{(1+bN)^3},
$$

its multiplier is

$$
F'(N_*)=\frac{2-\sqrt r}{\sqrt r}=\frac2{\sqrt r}-1.
$$

For every $r>1$, $-1<F'(N_*)<1$, so [fixed point stability for an iteration](../../../../../fixed-point-stability-for-an-iteration.md) proves that $N_*$ is **locally asymptotically stable**.

Scale the population by $x_\tau=bN_\tau$. Then

$$
x_{\tau+1}=f(x_\tau),\qquad f(x)=\frac{rx}{(1+x)^2}.
$$

The map increases on $0<x<1$, decreases on $x>1$, and has global maximum $f(1)=r/4$. Starting from $x_1=1$ therefore gives

$$
x_2=\frac r4=:U,
\qquad
x_3=f(U)=\frac{4r^2}{(4+r)^2}=:L.
$$

For $r>4$, writing $s=\sqrt r>2$ gives

$$
L-1=\frac{(s-2)(s+2)(3s^2+4)}{(s^2+4)^2}>0,
\qquad
(s-1)-L=\frac{(s-2)^3(s^2+s+2)}{(s^2+4)^2}>0.
$$

Thus $1<L<N_*b=s-1<U$. Since $f$ decreases on $[L,U]$, $f(U)=L$ and $f(L)>f(s-1)=s-1>L$, while the global maximum gives $f(L)\leq U$. Hence $f([L,U])\subseteq[L,U]$. The [cobweb plot](../../../../../cobweb-plot.md) consequently remains in this invariant interval after the first iterate, and both endpoints are attained at $\tau=2,3$:

$$
\boxed{\frac{4r^2}{(4+r)^2b}\leq N_\tau\leq\frac r{4b}\qquad(\tau\geq2).}
$$

The printed bound cannot include $\tau=1$, because $N_1=1/b<L/b$ when $r>4$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

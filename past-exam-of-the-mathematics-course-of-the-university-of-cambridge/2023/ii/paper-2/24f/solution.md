<h1 id="24f/solution">Solution</h1>

↑ **Parent:** [24F](../24f.md)

If $F:X\to Y$ is a nonconstant [holomorphic map](../../../../../holomorphic-map.md) between compact connected [Riemann surfaces](../../../../../riemann-surfaces.md), its [local degree](../../../../../local-degree-of-a-holomorphic-map.md) at $p$ is the integer $m_F(p)\geq1$ for which suitable local coordinates give

$$
F(z)-F(p)=az^{m_F(p)}+O(z^{m_F(p)+1}),
\qquad a\ne0.
$$

The [valency theorem](../../../../../valency-theorem.md) states that

$$
\sum_{p\in F^{-1}(y)}m_F(p)
$$

is independent of $y\in Y$. This common value is the [degree of a holomorphic map](../../../../../degree-of-a-holomorphic-map.md), denoted $\deg F$.

Now let $f$ be a nonconstant [rational function](../../../../../rational-function.md) of degree $d$. If its distinct finite [poles](../../../../../pole.md) have orders $m_1,\ldots,m_r$, and its pole order at infinity is $m_\infty\geq0$, then

$$
d=m_1+\cdots+m_r+m_\infty.
$$

The [derivative](../../../../../derivative.md) $f'$ has a pole of order $m_j+1$ at each finite pole. When $m_\infty>0$, the expansion $f(z)\sim cz^{m_\infty}$ shows that $f'(z)\sim cm_\infty z^{m_\infty-1}$ at infinity. Hence the [degree of the derivative of a rational function](../../../../../degree-of-the-derivative-of-a-rational-function.md) is

$$
\deg f'=
\begin{cases}
d+r-1,&m_\infty>0,\\
d+r,&m_\infty=0.
\end{cases}
$$

In the first case $r\geq0$, while in the second $1\leq r\leq d$; therefore

$$
\boxed{d-1\leq\deg f'\leq2d.}
$$

For every $d\geq1$, the lower bound is attained by $f(z)=z^d$, whose derivative has degree $d-1$ (with a constant assigned degree zero). For distinct $a_1,\ldots,a_d$, the function

$$
f(z)=\sum_{j=1}^d\frac1{z-a_j}
$$

has $d$ simple poles, degree $d$, and a derivative with $d$ double poles, so $\deg f'=2d$. Thus both rational bounds are sharp for every $d$.

Let next $g$ be a nonconstant [elliptic function](../../../../../elliptic-function.md) for the [period lattice](../../../../../period-lattice.md) $\Lambda$. Its [degree](../../../../../degree-of-an-elliptic-function.md) is the total order of its poles in a [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md); by the valency theorem, this is also the degree of the induced map $\mathbb C/\Lambda\to\widehat{\mathbb C}$. If these poles have orders $n_1,\ldots,n_s$, then $d=\deg g=\sum_jn_j$, and $g'$ has poles of orders $n_j+1$. The [degree of the derivative of an elliptic function](../../../../../degree-of-the-derivative-of-an-elliptic-function.md) is consequently

$$
\deg g'=d+s.
$$

Since every nonconstant elliptic function has at least one pole and $1\leq s\leq d$,

$$
\boxed{d+1\leq\deg g'\leq2d.}
$$

Let $d\geq3$ be odd. The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) supplies the lower-bound example

$$
g(z)=\wp(z)^{(d-3)/2}\wp'(z).
$$

It has one pole modulo $\Lambda$, of order $d$, so its derivative has one pole of order $d+1$. For the upper bound, choose distinct points $a_1,\ldots,a_d$ modulo $\Lambda$ and nonzero constants $c_j$ with $\sum_jc_j=0$. The quasi-periodicity of the [Weierstrass zeta function](../../../../../weierstrass-zeta-function.md) makes

$$
g(z)=\sum_{j=1}^dc_j\zeta(z-a_j)
$$

elliptic. It has exactly $d$ simple poles, while $g'$ has $d$ double poles. Therefore the two bounds are attained for every required odd degree.

## ↑ Ancestors (10)

1. [24F](../24f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

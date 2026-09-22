<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

The standard positive-cost interpretation requires $a>0$ and $a_0\ge0$. These signs are not printed. Without them the claim of a unique positive fixed point is false: $a=a_0=\lambda=0$ gives $f(z)=0$, with no positive fixed point. The following derivation gives the intended result under those cost assumptions; $b_0$ may be any finite constant.

Let $V_n(x)$ be the value with $n$ stages remaining. Starting from $V_0(x)=\frac12a_0x^2+b_0$, the [Bellman equation](../../../../../bellman-equation.md) is

$$
V_n(x)=\min_u\left\{\tfrac12(u^2+ax^2)+\beta\mathbb E V_{n-1}(\lambda x+u+\varepsilon)\right\}.
$$

If $V_{n-1}(x)=\frac12a_{n-1}x^2+b_{n-1}$, the minimized expression is a quadratic in $u$ with positive leading coefficient $1+\beta a_{n-1}$. Its derivative vanishes at $u=k_nx$, and completing the square gives

$$
\boxed{k_n=-\frac{\beta\lambda a_{n-1}}{1+\beta a_{n-1}},\quad a_n=a+\frac{\beta\lambda^2a_{n-1}}{1+\beta a_{n-1}},\quad b_n=\beta b_{n-1}+\tfrac12\beta\sigma^2a_{n-1}.}
$$

Induction establishes the value form and the control $u_j=k_{T-j}X_j$. Only zero mean and variance $\sigma^2$ of the independent noise were needed.

The [Riccati recurrence](../../../../../discrete-riccati-recurrence.md) fixed-point equation becomes

$$
\beta z^2+(1-a\beta-\beta\lambda^2)z-a=0.
$$

The product of its roots is $-a/\beta<0$, so exactly one is positive:

$$
\boxed{a_* =\frac{a\beta+\beta\lambda^2-1+\sqrt{(1-a\beta-\beta\lambda^2)^2+4a\beta}}{2\beta}.}
$$

For $z\ge0$, $f'(z)=\beta\lambda^2/(1+\beta z)^2\ge0$, while $f(z)-z$ is positive below $a_*$ and negative above it. Monotonicity of $f$ prevents overshooting the fixed point. Thus $a_n$ increases to $a_*$ if $a_0<a_*$, decreases to it if $a_0>a_*$, and is constant if $a_0=a_*$. Continuity identifies the limit uniquely.

Iteration of the second recurrence gives $b_n=\beta^nb_0+\frac12\beta\sigma^2\sum_{j=0}^{n-1}\beta^{n-1-j}a_j$. Subtract the same expression with every $a_j$ replaced by $a_*$. The early finite part vanishes geometrically, and the later part is bounded by $\sup_{j\ge J}|a_j-a_*|/(1-\beta)$ times the fixed factor. Taking $n\to\infty$, then $J\to\infty$, proves

$$
\boxed{b_n\to\frac{\beta\sigma^2a_*}{2(1-\beta)},\qquad k_n\to-\frac{\beta\lambda a_*}{1+\beta a_*}.}
$$

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

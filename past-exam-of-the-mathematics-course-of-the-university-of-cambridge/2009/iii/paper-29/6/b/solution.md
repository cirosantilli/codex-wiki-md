<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $\gamma=1-2a\ne0$ and interpret the positive solution up to its first hit of zero, where the displayed drift is singular. For $s(x)=x^\gamma$,

$$
s'(x)=\gamma x^{\gamma-1},\qquad s''(x)=\gamma(\gamma-1)x^{\gamma-2},\qquad\frac12s''+\frac ax s'=\gamma\left(\frac{\gamma-1}2+a\right)x^{\gamma-2}=0.
$$

Thus $s$ is a [scale function of a one-dimensional diffusion](../../../../../../scale-function-stochastic-processes.md) on every $[\varepsilon,\infty)$ with $\varepsilon>0$. It is strictly decreasing if $a>1/2$; multiplying by $-1$ gives the conventionally increasing scale, without changing any hitting ratio.

Fix $0<\varepsilon<x<R$. Exit from $(\varepsilon,R)$ is almost surely finite. Indeed the coefficients are locally Lipschitz there, so there is no lifetime obstruction in this compact interval. If the process stayed inside forever, the equation and $a/X>0$ would give $B_t\leq R-x$ for every $t$, contradicting the almost sure unboundedness above of [Brownian motion](../../../../../../brownian-motion-split.md). Therefore part (a)'s bounded optional-stopping argument applies and gives

$$
\mathbb P_x(T_\varepsilon<T_R)=\frac{x^\gamma-R^\gamma}{\varepsilon^\gamma-R^\gamma},\qquad\mathbb P_x(T_R<T_\varepsilon)=\frac{x^\gamma-\varepsilon^\gamma}{R^\gamma-\varepsilon^\gamma}.
$$

If $a>1/2$, then $\gamma<0$ and $\varepsilon^\gamma\to\infty$, so $\mathbb P_x(T_\varepsilon<T_R)\to0$. Hitting zero before $R$ would entail hitting every $\varepsilon$ before $R$; it therefore has probability zero. Every continuous path reaching zero in finite time is bounded up to that time, so it belongs to this event for some integer $R>x$. A countable union proves

$$
\boxed{a>\tfrac12\quad\Longrightarrow\quad T_0=\infty\text{ almost surely}.}
$$

If $0<a<1/2$, then $\gamma\in(0,1)$. Taking $\varepsilon\downarrow0$ in the probabilities alone does not yet exclude approaching zero only at infinite time. To establish [finite-time access to zero for Bessel dimensions below two](../../../../../../finite-time-access-to-zero-for-bessel-dimensions-below-two.md), define

$$
v_R(y)=\frac{R^{2-\gamma}y^\gamma-y^2}{1+2a}\qquad(0\leq y\leq R).
$$

It is continuous, nonnegative, zero at $0,R$, and satisfies $\mathcal Lv_R=-1$ on $(0,R)$, since $\mathcal L(y^\gamma)=0$ and $\mathcal L(y^2)=1+2a$. Itô's formula stopped at $\tau_{\varepsilon,R}=T_\varepsilon\wedge T_R$, followed first by expectation at $t\wedge\tau_{\varepsilon,R}$, gives

$$
\mathbb E(t\wedge\tau_{\varepsilon,R})=v_R(x)-\mathbb E v_R(X_{t\wedge\tau_{\varepsilon,R}})\leq v_R(x).
$$

Let $t\to\infty$ and then $\varepsilon\downarrow0$. The [stopping times](../../../../../../stopping-time.md) increase and have uniformly bounded expectation, so their limit $\tau_{0,R}$ is finite almost surely. On this finite interval $X\leq R$, and the increasing drift integral is bounded by $R-x-\inf_{u\leq\tau_{0,R}}B_u$. Hence it has a finite limit, and the stochastic equation makes $X$ extend continuously to $\tau_{0,R}$. If the upper endpoint was not reached, the lower stopped values tend to zero, so the terminal value is zero. Thus $\tau_{0,R}=T_0\wedge T_R$ genuinely denotes a finite hitting time.

The lower-exit events decrease to $\{T_0<T_R\}$ as $\varepsilon\downarrow0$, giving $\mathbb P_x(T_0<T_R)=1-(x/R)^\gamma$. Let $R\to\infty$ to obtain

$$
\boxed{0<a<\tfrac12\quad\Longrightarrow\quad\mathbb P_x(T_0<\infty)=1.}
$$

There is no finite explosion to $+\infty$: on a finite horizon, any excursion above level $1$ has drift at most $a$, so its height is bounded by $\max\{x,1\}+2\sup_{u\leq t}|B_u|+at$. The two alternatives therefore describe the zero-boundary lifetime, giving the [Hitting-zero classification for a Bessel process](../../../../../../hitting-zero-classification-for-a-bessel-process.md) of dimension $2a+1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\phi(u)=\int e^{iuy}\mu(dy)$. Since $1-\cos(uy)\geq0$, the [Tonelli theorem](../../../../../tonelli-theorem.md) gives

$$
\lambda\int_0^{1/\lambda}(1-\operatorname{Re}\phi(u))\,du
=\int_{\mathbb R}\left(1-\frac{\sin(y/\lambda)}{y/\lambda}\right)\mu(dy),
$$

with the fraction defined to be one at zero. For $|x|\geq1$, $\sin x/x\leq\sin1$. To verify the constant, the function is even; on $[1,\pi]$ it decreases because $(x\cos x-\sin x)'=-x\sin x<0$ on $(0,\pi)$ and $x\cos x-\sin x$ starts from zero. On $[\pi,\infty)$, $\sin x/x\leq1/\pi<\sin1$. Consequently the integrand is at least $1-\sin1$ on $|y|\geq\lambda$, proving the [characteristic-function tail bound](../../../../../characteristic-function-tail-bound.md)

$$
\boxed{\mu(|y|\geq\lambda)\leq\frac{\lambda}{1-\sin1}\int_0^{1/\lambda}(1-\operatorname{Re}\phi(u))\,du.}
$$

For pointwise convergence $\phi_n\to\phi$, where $\phi$ is a [characteristic function](../../../../../characteristic-function.md), the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) applies on each finite integration interval, since the integrands lie between zero and two. Hence

$$
\limsup_{n\to\infty}\mu_n(|y|\geq\lambda)
\leq\frac{1}{1-\sin1}\int_0^1(1-\operatorname{Re}\phi(v/\lambda))\,dv.
$$

Continuity of $\phi$ at zero and $\phi(0)=1$ make the right side tend to zero as $\lambda\to\infty$. Given $\varepsilon>0$, choose $\lambda$ so it is below $\varepsilon/2$. The tail [probability](../../../../../probability.md) is then below $\varepsilon$ for all sufficiently large $n$. Enlarge the compact interval to control the finitely many remaining measures, each of which has vanishing tails. This proves **uniform tightness of the entire sequence**, not just of its tail. It is the [characteristic-function tightness bound](../../../../../characteristic-function-tightness-bound.md) principle with the sharper displayed constant.

For the integrable mean-zero summands, differentiation at zero is justified by

$$
\left|\frac{e^{iuX_1}-1}{u}\right|\leq|X_1|,\qquad
\frac{e^{iuX_1}-1}{u}\longrightarrow iX_1.
$$

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives $\phi'(0)=i\mathbb E X_1=0$. Define

$$
\psi(u)=\begin{cases}|1-\phi(u)|/|u|,&u\ne0,\\0,&u=0.\end{cases}
$$

It is continuous away from zero by continuity of the [characteristic function](../../../../../characteristic-function.md), and continuous at zero by the zero derivative. Since $|\phi(u)|\leq1$, the finite [geometric series](../../../../../geometric-series.md) yields, for $n\geq1$,

$$
|1-\phi(u)^n|=|1-\phi(u)|\left|\sum_{j=0}^{n-1}\phi(u)^j\right|
\leq n|1-\phi(u)|,
$$

and the case $n=0$ has both sides zero. Thus the requested uniform-in-$n$ estimate is

$$
\boxed{|1-\phi(u)^n|\leq\psi(u)n|u|,\qquad\psi\text{ continuous},\quad\psi(0)=0.}
$$

This is the [characteristic-function derivative under an absolute first moment](../../../../../characteristic-function-derivative-under-an-absolute-first-moment.md) estimate.

[Independence](../../../../../independent-random-variables.md) makes the [characteristic function](../../../../../characteristic-function.md) of $S_n/n=(X_1+\cdots+X_n)/n$ equal to $\phi(u/n)^n$. Therefore $|1-\phi(u/n)^n|\leq|u|\psi(u/n)$. Applying the already proved [characteristic-function tail bound](../../../../../characteristic-function-tail-bound.md) to its distribution, for every $\varepsilon>0$,

$$
\mathbb P(|S_n/n|\geq\varepsilon)
\leq\frac{\varepsilon}{1-\sin1}\int_0^{1/\varepsilon}u\psi(u/n)\,du\longrightarrow0.
$$

The convergence follows because $\sup_{0\leq u\leq1/\varepsilon}\psi(u/n)\to0$, and the remaining integral of $u$ is finite. Hence $\boxed{S_n/n\to0\text{ in probability}}$, the mean-zero [weak law of large numbers](../../../../../weak-law-of-large-numbers.md). This deduction uses the tail bound directly and does not presuppose the [Lévy continuity theorem](../../../../../levy-continuity-theorem.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

One convenient version of [Watson's lemma](../../../../../../watson-s-lemma.md) is the following. Suppose $G(t)$ is integrable away from zero and has, as $t\downarrow0$, an [asymptotic expansion](../../../../../../asymptotic-expansion.md) $G(t)\sim\sum_{j\geq0}c_jt^{\beta+j-1}$, where $\beta>0$. On a finite interval, or on an infinite interval with suitable exponential growth control,

$$
\int_0^T e^{-\lambda t}G(t)\,dt\sim\sum_{j\geq0}\frac{c_j\Gamma(\beta+j)}{\lambda^{\beta+j}},\qquad \lambda\to+\infty.
$$

To prove a finite truncation, split the [integral](../../../../../../integral.md) at a fixed small $\delta>0$. The part away from zero is exponentially small. On $(0,\delta)$ subtract the first $N$ local terms and bound the remainder by $Ct^{\beta+N-1}$; its [integral](../../../../../../integral.md) is $O(\lambda^{-\beta-N})$. Extending each [polynomial](../../../../../../polynomial-split.md) [integral](../../../../../../integral.md) to infinity changes it only exponentially, and the substitution $u=\lambda t$ produces the [Gamma integral](../../../../../../gamma-integral.md). A little-o local remainder gives the corresponding little-o asymptotic remainder. This is a proof by localization and remainder bounds, rather than merely formal integration of a series.

For the monotone-phase [integral](../../../../../../integral.md), assume the [derivatives](../../../../../../derivative.md) needed below exist and are bounded near $a$, and the rest of the [integral](../../../../../../integral.md) is controlled. Put $t=\phi(a)-\phi(x)$. Since $\phi'(a)<0$, this is a regular endpoint coordinate and

$$
f(\lambda)=e^{\lambda\phi(a)}\int_0^{\phi(a)-\phi(b)}e^{-\lambda t}G(t)\,dt,\qquad G(t)=-\frac{g(x(t))}{\phi'(x(t))}.
$$

Differentiating with $dx/dt=-1/\phi'$ gives $G(0)=-g(a)/\phi'(a)$ and $G'(0)=g'(a)/\phi'(a)^2-g(a)\phi''(a)/\phi'(a)^3$. [Watson's lemma](../../../../../../watson-s-lemma.md) therefore gives the [two-term monotone-endpoint Laplace expansion](../../../../../../two-term-monotone-endpoint-laplace-expansion.md)

$$
\boxed{f(\lambda)\sim e^{\lambda\phi(a)}\left[-\frac{g(a)}{\lambda\phi'(a)}+\frac1{\lambda^2}\left(\frac{g'(a)}{\phi'(a)^2}-\frac{g(a)\phi''(a)}{\phi'(a)^3}\right)\right].}
$$

An $O(e^{\lambda\phi(a)}\lambda^{-3})$ remainder follows, for example, from a sufficiently smooth transformed amplitude with bounded second [derivative](../../../../../../derivative.md) near zero. The displayed second coefficient can vanish for special amplitudes without changing the expansion.

The unheaded transition request concerns a [cubic endpoint-to-saddle transition](../../../../../../cubic-endpoint-to-saddle-transition.md). Near $x=0$ its exponent has the expansion

$$
-x+\alpha\sin x=-(1-\alpha)x-\frac{\alpha x^3}{6}+O(x^5).
$$

At the cubic endpoint $x$ has size $\lambda^{-1/3}$. Requiring the linear term to contribute on the same scale gives $1-\alpha=O(\lambda^{-2/3})$. Thus the [distinguished limit](../../../../../../distinguished-limit.md) and its uniform leading [integral](../../../../../../integral.md) are

$$
\boxed{p=\frac23,\qquad q=\frac13,\qquad h(\nu)=\int_0^\infty e^{-\nu t-t^3/6}\,dt,\qquad f(\lambda,1-\nu\lambda^{-2/3})\sim\lambda^{-1/3}h(\nu).}
$$

For fixed $\nu$, the substitution $x=\lambda^{-1/3}t$ makes the omitted exponent terms $O(\lambda^{-2/3})$ on bounded $t$ intervals. Cubic decay controls the remaining tail, while the original interval away from zero is exponentially negligible. The estimate is uniform for $\nu$ in compact sets. In the printed range $\alpha\leq1$, $\nu\geq0$; the same transition [integral](../../../../../../integral.md) also makes sense for negative fixed $\nu$.

At $\nu=0$, the [Gamma integral](../../../../../../gamma-integral.md) gives $h(0)=6^{1/3}\Gamma(1/3)/3$, recovering the cubic endpoint regime. For $\nu\to+\infty$, scale $t=u/\nu$ and expand $e^{-u^3/(6\nu^3)}$ to obtain $h(\nu)=\nu^{-1}-\nu^{-4}+O(\nu^{-7})$. Its leading term gives $\lambda^{-1/3}/\nu=1/[\lambda(1-\alpha)]$, recovering the ordinary endpoint regime in their overlap. Both matching limits are therefore checked explicitly.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

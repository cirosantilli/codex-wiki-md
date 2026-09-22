<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The original PDF specifies a bounded solution class $C_b^2$, rather than the $C_0^2$ transcribed in the TeX. Write $\phi(x)=\min(1,\max(0,-x))$ and fix a time $t>0$. For Brownian motion starting at $x$, consider

$$
F_s=\exp\left(-\lambda\int_0^s\phi(B_r)dr\right)u(t-s,B_s),\qquad0\leq s\leq t.
$$

The [Itô formula](../../../../../ito-s-lemma.md) and ordinary product rule give a drift proportional to $-u_t+\tfrac12u_{xx}-\lambda\phi u$, which vanishes by the equation. Therefore $F$ is a local martingale. It is bounded on this horizon because $u$ is bounded and $\phi\geq0$, so the [bounded local martingale criterion](../../../../../bounded-local-martingale-criterion.md) makes it a true martingale. Its endpoint values are $F_0=u(t,x)$ and $F_t=e^{-\lambda\int_0^t\phi(B_r)dr}$, using $u(0,\cdot)=1$. Consequently

$$
\boxed{u^\lambda(t,x)=\mathbb E_x\exp\left(-\lambda\int_0^t\phi(B_s)ds\right).}
$$

This proves the required [Feynman-Kac formula with a bounded potential](../../../../../feynman-kac-formula-with-a-bounded-potential.md) directly, and also gives uniqueness within the stated bounded solution class.

Let $I=\int_0^t\phi(B_s)ds$. By [dominated convergence](../../../../../dominated-convergence-theorem.md), $e^{-\lambda I}\to\mathbf1_{\{I=0\}}$ in expectation. Continuity of $B$ and $\phi$ shows that $I=0$ exactly when $B_s\geq0$ throughout $[0,t]$: a negative value at any time produces a nontrivial interval with positive integrand. For $x<0$ such an interval occurs immediately, so the limiting probability is zero. For $x>0$, the [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) and the atom-free distribution of the running minimum give

$$
\mathbb P_x(\min_{s\leq t}B_s\geq0)=1-2\mathbb P_x(B_t\leq0).
$$

For $x=0$ this probability is zero: the reflection formula for levels $-\varepsilon$, followed by $\varepsilon\downarrow0$, shows that Brownian motion goes below zero before $t$ almost surely. Thus

$$
\boxed{\lim_{\lambda\to\infty}u^\lambda(t,x)=\begin{cases}1-2\mathbb P_x(B_t\leq0),&x\geq0,\\0,&x<0.\end{cases}}
$$

This is the [soft killing limit for Brownian nonnegative survival](../../../../../soft-killing-limit-for-brownian-nonnegative-survival.md). The assertion is pointwise for positive time, as requested; no claim of uniform convergence across the initial-time boundary is needed.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

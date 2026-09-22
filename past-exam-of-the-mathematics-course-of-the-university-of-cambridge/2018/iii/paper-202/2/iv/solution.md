<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

On the right-hand side, $\mathbb E_x$ means that the reference [Brownian motion](../../../../../../brownian-motion-split.md) starts at $B_0=x$; on the left it means the [stochastic differential equation](../../../../../../stochastic-differential-equation.md) starts at $X_0=x$. Since $h$ is smooth and compactly supported, $h'$ is bounded and globally [Lipschitz continuous](../../../../../../lipschitz-continuity.md). Define the [stochastic exponential](../../../../../../doleans-dade-exponential.md)

$$
D_t=\exp\!\left(\int_0^t h'(B_s)\,dB_s-\frac12\int_0^t h'(B_s)^2\,ds\right).
$$

The [Novikov condition](../../../../../../novikov-s-condition.md) holds on every finite horizon $T$, because $\mathbb E\exp(\frac12\int_0^Th'(B_s)^2ds)\leq\exp(T\|h'\|_\infty^2/2)$. Thus $D$ is a true [martingale](../../../../../../martingale-split.md). Under $d\mathbb Q=D_Td\mathbb P$, the [Girsanov theorem](../../../../../../girsanov-theorem.md) makes $\widehat B_t=B_t-x-\int_0^th'(B_s)ds$ a standard [Brownian motion](../../../../../../brownian-motion-split.md) for $t\leq T$. Consequently $B$ under $\mathbb Q$ solves the prescribed [stochastic differential equation](../../../../../../stochastic-differential-equation.md); the [existence and pathwise uniqueness theorem for a stochastic differential equation](../../../../../../existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation.md) identifies its law with that of $X$.

The [Itô formula](../../../../../../ito-s-lemma.md) gives $\int_0^t h'(B_s)dB_s=h(B_t)-h(x)-\frac12\int_0^th''(B_s)ds$. Hence, for any bounded measurable $f$,

$$
\boxed{\mathbb E_xf(X_t)=\mathbb E_x\!\left[\exp\!\left(h(B_t)-h(x)-\int_0^tV(B_s)\,ds\right)f(B_t)\right],\quad V=\frac12(h')^2+\frac12h''.}
$$

The finite-horizon argument applies separately to every $t\geq0$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

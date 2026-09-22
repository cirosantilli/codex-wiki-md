<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

If the urn contains $g$ green balls, it contains $g+2$ red balls: both update rules preserve the difference $R-G=2$. Until absorption at $g=0$, the green count is therefore a birth-death chain with

$$
p_g=\mathbb P(g\to g-1)=\frac{g}{2g+2},
\qquad
q_g=\mathbb P(g\to g+1)=\frac{g+2}{2g+2}.
$$

The [function](../../../../../function-split.md)

$$
h(g)=\frac1{g+1}
$$

is harmonic, since

$$
p_gh(g-1)+q_gh(g+1)
=\frac1{2(g+1)}+\frac1{2(g+1)}=h(g).
$$

Let $\tau_0$ and $\tau_N$ be the hitting times of $0$ and $N$. The [optional sampling theorem for a supermartingale](../../../../../optional-sampling-theorem-for-a-supermartingale.md), applied to the bounded stopped martingale $h(G_{n\wedge\tau_0\wedge\tau_N})$, gives

$$
h(m)=\mathbb P_m(\tau_0<\tau_N)
+\frac1{N+1}\mathbb P_m(\tau_N<\tau_0).
$$

Solving,

$$
\mathbb P_m(\tau_0<\tau_N)
=\frac{N-m}{N(m+1)}.
$$

Letting $N\to\infty$, the events on the left increase to eventual termination. The [harmonic hitting probability for the balanced-difference urn](../../../../../harmonic-hitting-probability-for-the-balanced-difference-urn.md) is therefore

$$
\boxed{\mathbb P(\text{the process terminates})=\frac1{m+1}}.
$$

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

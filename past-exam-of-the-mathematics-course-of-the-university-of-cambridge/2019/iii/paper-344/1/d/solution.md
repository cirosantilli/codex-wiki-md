<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose an even positive $J(q)$. Each independent complex [Fourier mode](../../../../../../fourier-mode.md) of the real field has density $(J(q)/\pi)e^{-J(q)|\phi_q|^2}$, so

$$
\langle\phi_q\phi_p\rangle_0=\frac{\delta_{p,-q}}{J(q)}.
$$

The quadratic part therefore has expectation $\sum_q^+G(q)/J(q)$. For the quartic part, apply [Isserlis theorem](../../../../../../isserlis-s-theorem.md) to its four jointly centered [Gaussian random variables](../../../../../../gaussian-random-variable.md), or to their real and imaginary components. Pairing the two differentiated fields together imposes $q_2=-q_1$, and its contribution is

$$
\frac BV\left(\sum_q\frac{q^2}{J(q)}\right)\left(\sum_p\frac1{J(p)}\right).
$$

Each of the two other pairings instead gives $-(B/V)|\sum_q q/J(q)|^2=0$, because the summand is odd under $q\mapsto-q$. Thus only the displayed contribution remains. Each full sum is twice its [positive-wavevector sum for a real field](../../../../../../positive-wavevector-sum-for-a-real-field.md); putting $S_0=\sum_q^+1/J(q)$ and $S_2=\sum_q^+q^2/J(q)$ gives $\langle H_4\rangle_0=4BS_2S_0/V$.

Substitute these expectations, $F_0$ and $\langle H_0\rangle_0$ into the [Feynman-Bogoliubov inequality](../../../../../../gibbs-bogoliubov-feynman-inequality.md):

$$
\boxed{F\leq\mathcal F[J]=\sum_q^+\left[\log\frac{J(q)}\pi-1+\frac{G(q)}{J(q)}\right]+\frac{4B}{V}S_2S_0.}
$$

The zero mode is absent by the composition constraint. The counting uses one representative of every nonzero $\{q,-q\}$ pair, so no extra factor of two is assigned to an independent complex amplitude.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

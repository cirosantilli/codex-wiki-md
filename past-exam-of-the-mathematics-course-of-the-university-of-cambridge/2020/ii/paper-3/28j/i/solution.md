<h1 id="28j/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $K(t,\mathord\cdot)$ be the [Markov kernel](../../../../../../markov-kernel.md) of the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md). Away from the possibility of remaining at $t$, its transition density is

$$
k(t,s)=q(s\mid t)\rho(t,s).
$$

Multiplication by the target density gives

$$
\begin{aligned}
\mu(t)k(t,s)
&=\mu(t)q(s\mid t)
\min\left\{\frac{\mu(s)q(t\mid s)}{\mu(t)q(s\mid t)},1\right\}\\
&=\min\{\mu(s)q(t\mid s),\mu(t)q(s\mid t)\}\\
&=\mu(s)k(s,t).
\end{aligned}
$$

This is [detailed balance](../../../../../../detailed-balance.md) for every pair of distinct states.

Write

$$
r(t)=1-\int_\Theta k(t,s)\,ds
$$

for the rejection probability, so

$$
K(t,ds)=k(t,s)\,ds+r(t)\delta_t(ds).
$$

For every measurable $B\subseteq\Theta$, detailed balance and the [Tonelli theorem](../../../../../../tonelli-theorem.md) give

$$
\begin{aligned}
\int_\Theta K(t,B)\mu(t)\,dt
&=\int_B\int_\Theta \mu(t)k(t,s)\,dt\,ds
 +\int_B\mu(t)r(t)\,dt\\
&=\int_B\mu(s)\left[\int_\Theta k(s,t)\,dt+r(s)\right]ds\\
&=\int_B\mu(s)\,ds.
\end{aligned}
$$

**Hence $\mu$ is an [invariant distribution](../../../../../../stationary-distribution.md) of the chain.**

## ↑ Ancestors (11)

1. [I](../i.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\widetilde\pi$ be a nonnegative target kernel and $q(y\mid x)$ a [proposal distribution](../../../../../../proposal-distribution.md). At state $x$, propose $Y\sim q(\cdot\mid x)$, draw an independent uniform $U$, and move to $Y$ if

$$
\boxed{U\leq\alpha(x,Y),\qquad\alpha(x,y)=\min\left(1,\frac{\widetilde\pi(y)q(x\mid y)}{\widetilde\pi(x)q(y\mid x)}\right).}
$$

Otherwise keep $x$. This is the [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md). Start on the positive target support, with the usual zero-ratio conventions. The unknown [normalizing constant](../../../../../../normalizing-constant.md) cancels.

An unnormalized kernel is sufficient, provided $0<\int\widetilde\pi<\infty$. A genuinely improper target with infinite integral is not a probability density and cannot supply a stationary target probability distribution. The acceptance formula can still be written formally, but cannot be said to generate samples from that nonexistent probability law.

Because rejected proposals leave the state unchanged, the [Markov kernel](../../../../../../markov-kernel.md) includes an atom:

$$
K(x,dy)=q(y\mid x)\alpha(x,y)\,dy+r(x)\delta_x(dy),\quad
r(x)=1-\int q(y\mid x)\alpha(x,y)\,dy.
$$

[Detailed balance](../../../../../../detailed-balance.md) with a probability measure $\pi$ means the measure identity

$$
\boxed{\pi(dx)K(x,dy)=\pi(dy)K(y,dx).}
$$

Where both sides have ordinary densities, this reads $\pi(x)K(x,y)=\pi(y)K(y,x)$. The measure formulation also includes the rejection atom. Integrating it shows that $\pi$ is invariant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

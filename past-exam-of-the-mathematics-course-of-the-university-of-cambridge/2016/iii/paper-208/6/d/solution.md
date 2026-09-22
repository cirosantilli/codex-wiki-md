<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md): for an [invariant distribution](../../../../../../stationary-distribution.md) $\pi$ and an integrable function $h$, the time average converges almost surely to $\int h\,d\pi$ under the usual ergodicity conditions. This is the relevant theorem for correlated [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) output, rather than the [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md). Here $h(x)=x_1$ is integrable. Indeed, putting

$$
V(x)=x_1^2x_2^2+x_1^2+x_2^2-8x_1-8x_2,
$$

we have $V(x)\geq(x_1-4)^2+(x_2-4)^2-32$, which bounds the unnormalized density by a constant times an integrable Gaussian density and also gives finite first moments.

For a proposal scale $s>0$, initialize $X_0$ anywhere in $\mathbb R^2$. At each step draw [independent random variables](../../../../../../independent-random-variables.md) $Z_1,Z_2$ with the [standard normal distribution](../../../../../../standard-normal-distribution.md) and an independent uniform $U$, propose $Y=X_t+s(Z_1,Z_2)$, and accept when

$$
\boxed{\log U\leq\min\{0,-\tfrac12(V(Y)-V(X_t))\}.}
$$

Otherwise set $X_{t+1}=X_t$. The normal proposal is symmetric, so its density cancels; the target [normalizing constant](../../../../../../normalizing-constant.md) $c$ also cancels. Include every state in the average, including repeated states after rejection. The [ergodic theorem for a positive Harris recurrent Markov chain](../../../../../../ergodic-theorem-for-a-positive-harris-recurrent-markov-chain.md) then gives

$$
\boxed{N^{-1}\sum_{t=1}^NX_{t,1}\longrightarrow E_\pi X_1\quad\text{almost surely}.}
$$

A fixed discarded initial segment does not change this limit.

Small proposal [variance](../../../../../../variance-split.md) gives high acceptance but tiny moves and strong serial dependence. Large [variance](../../../../../../variance-split.md) gives more ambitious moves, but many proposals enter very low-density regions and are rejected, creating long runs at one state. An intermediate scale should be assessed by exploration and [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md), not acceptance rate alone.

This density has two modes, at $(2+\sqrt3,2-\sqrt3)$ and their interchange. To see this, stationary points satisfy $x_1(1+x_2^2)=x_2(1+x_1^2)=4$, implying either $x_1=x_2$ or $x_1x_2=1$. The unequal solutions have $x_1+x_2=4$ and are local minima of $V$; the equal solution is a saddle. Mode switching is therefore a material part of proposal-scale selection: a chain confined to one mode can have high acceptance and a misleading finite-run estimate.

<a id="6/d/image-two-modes-of-the-quartic-target-density-with-the-diagonal-saddle-between-them-explaining-slow-mode-switching-in-random-walk-metropolis-hastings"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208-quartic-modes.png)

**[Figure 1](#6/d/image-two-modes-of-the-quartic-target-density-with-the-diagonal-saddle-between-them-explaining-slow-mode-switching-in-random-walk-metropolis-hastings). Two modes of the quartic target density, with the diagonal saddle between them, explaining slow mode switching in random-walk Metropolis-Hastings**.

## ↑ Ancestors (11)

1. [D](../d.md)
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

<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Both [Poisson processes](../../../../../../poisson-process.md) start at zero and have càdlàg paths. On disjoint time intervals their increments are independent, and [independence](../../../../../../independent-random-variables.md) of the two processes makes the difference increments independent as well. Their increment laws depend only on interval length, so $X$ has [stationary increments](../../../../../../stationary-increments.md). For a time interval of length $h$, the probability that either Poisson process has a jump is $1-e^{-h}\to0$. This proves [stochastic continuity](../../../../../../stochastic-continuity.md). Consequently **the difference is a Lévy process**, equivalently a [continuous-time symmetric simple random walk](../../../../../../continuous-time-symmetric-simple-random-walk.md) with total jump rate one and jumps $+1$ and $-1$ each chosen with probability $1/2$.

The [characteristic function](../../../../../../characteristic-function.md) of a Poisson variable of mean $\lambda$ is $\exp\{\lambda(e^{i\theta}-1)\}$. [Independence](../../../../../../independent-random-variables.md) therefore gives

$$
\mathbb E e^{i\theta X_t}
=\exp\left\{\frac t2(e^{i\theta}-1)+\frac t2(e^{-i\theta}-1)\right\}
=\exp\{t(\cos\theta-1)\}.
$$

Thus, in the negative-exponent convention of part (a),

$$
\boxed{\psi(\theta)=1-\cos\theta.}
$$

In the positive-exponent convention the answer is $\widetilde\psi(\theta)=\cos\theta-1$. The [Compound Poisson process](../../../../../../compound-poisson-process.md) has mean zero and [variance](../../../../../../variance-split.md) $t$, consistent with the expansion $\psi(\theta)=\theta^2/2+O(\theta^4)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

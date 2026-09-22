<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the [Poisson distribution](../../../../../poisson-distribution.md) with [probability mass function](../../../../../probability-mass-function.md) $\pi_n=e^{-\lambda}\lambda^n/n!$ on $\mathbb N_0$. A symmetric nearest-neighbour proposal with a reflecting boundary is

$$
q(n,n+1)=\tfrac12\quad(n\geq0),\qquad q(n,n-1)=\tfrac12\quad(n\geq1),\qquad q(0,0)=\tfrac12.
$$

All other entries vanish. In particular, the boundary proposal does not force a move to one: retaining the [probability](../../../../../probability.md) $q(0,0)=1/2$ makes $q(0,1)=q(1,0)$.

The adjacent ratios of the [Poisson distribution](../../../../../poisson-distribution.md) are $\pi_{n+1}/\pi_n=\lambda/(n+1)$ and $\pi_{n-1}/\pi_n=n/\lambda$. The [Metropolis–Hastings acceptance probability](../../../../../metropolis-hastings-acceptance-probability.md) consequently gives

$$
u_n=\tfrac12\min\{1,\lambda/(n+1)\},\qquad d_n=\tfrac12\min\{1,n/\lambda\}\ (n\geq1),\qquad d_0=0,
$$

where the symbol $u_n$ denotes the upward [transition probability](../../../../../transition-probability.md). Thus the complete [transition matrix](../../../../../stochastic-matrix.md) is

$$
\boxed{P(n,n+1)=u_n,\quad P(n,n-1)=d_n,\quad P(n,n)=1-u_n-d_n,}
$$

with no downward entry at zero and all other entries zero. In matrix form,

$$
P=\begin{pmatrix}
1-u_0&u_0&0&0&\cdots\\
d_1&1-u_1-d_1&u_1&0&\cdots\\
0&d_2&1-u_2-d_2&u_2&\cdots\\
\vdots&\vdots&\ddots&\ddots&\ddots
\end{pmatrix}.
$$

Every row is nonnegative and sums to one. An executable [Python](../../../../../python-programming-language.md) step of this [Poisson Metropolis chain](../../../../../poisson-metropolis-chain.md) is:

```
def poisson_step(n, lam, rng):
    if lam <= 0 or n < 0 or int(n) != n:
        raise ValueError("require lam > 0 and an integer n >= 0")
    y = n + 1 if rng.random() < 0.5 else max(0, n - 1)
    ratio = lam / (n + 1) if y > n else n / lam if y < n else 1.0
    return y if rng.random() < min(1.0, ratio) else n
```

Supply a [pseudorandom number generator](../../../../../pseudorandom-number-generator.md) such as `random.Random(2021)` and retain each returned state, including repeats. No [normalizing constant](../../../../../normalizing-constant.md) or evaluation of a [factorial](../../../../../factorial.md) is needed by the algorithm.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Bayesian statistical probabilistic programming](../../../bayesian-statistical-probabilistic-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)

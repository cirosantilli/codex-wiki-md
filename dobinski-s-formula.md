<h1 id="dobinski-s-formula">Dobiński's formula</h1>

↑ **Parent:** [Bell number](bell-number.md)

For $X$ with [Poisson distribution](poisson-distribution.md) of [mean](expected-value-split.md) one, every [factorial moment](factorial-moment.md) satisfies $\mathbb E[(X)_k]=1$. The [polynomial](polynomial-split.md) identity

$$
x^n=\sum_{k=0}^n S(n,k)(x)_k
$$

expresses powers in terms of [falling factorials](falling-factorial.md), where $S(n,k)$ are [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md). Substituting $X$ and using [linearity of expectation](linearity-of-expectation.md) proves

$$
\mathbb E[X^n]=\sum_{k=0}^n S(n,k)=B_n.
$$

On the other hand, the [probability mass function](probability-mass-function.md) gives $\mathbb E[X^n]=e^{-1}\sum_{j=0}^\infty j^n/j!$. This proves Dobiński's formula and explains why a count of [set partitions](set-partition.md) is a [moment](moment.md) of a [Poisson distribution](poisson-distribution.md). For example, $\mathbb E[X^3]=\mathbb E[(X)_3+3(X)_2+X]=1+3+1=5=B_3$. At $n=0$, take $j^0=1$ also for $j=0$, obtaining $B_0=1$. For each fixed $n$, the [ratio test](ratio-test.md) proves convergence of the displayed infinite sum.

## ↑ Ancestors (7)

1. [Bell number](bell-number.md)
2. [Stirling numbers of the second kind](stirling-numbers-of-the-second-kind.md)
3. [Set partition](set-partition.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2015/prelims/mathematics-iii/5/b/iv/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/discrete-mathematics-continuous-mathematics-and-probability/8/b/iv/solution.md)

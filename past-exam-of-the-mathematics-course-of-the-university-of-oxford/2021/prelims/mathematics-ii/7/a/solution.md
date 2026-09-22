<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $f:[a,b]\to\mathbb R$ be a bounded [function](../../../../../../function-split.md), with $a<b$. A [partition of an interval](../../../../../../partition-of-an-interval.md) is $\mathcal P=(a=x_0<x_1<\cdots<x_N=b)$; its [mesh of a partition](../../../../../../mesh-of-a-partition.md) is $\|\mathcal P\|=\max_i(x_i-x_{i-1})$. Choose arbitrary tags $\xi_i\in[x_{i-1},x_i]$. The corresponding [Riemann sum](../../../../../../riemann-sum.md) is

$$
\sum(f;\mathcal P,\vec\xi)=\sum_{i=1}^N f(\xi_i)(x_i-x_{i-1}).
$$

The [Riemann sum convergence theorem](../../../../../../riemann-sum-convergence-theorem.md) says that $f$ is [Riemann integrable](../../../../../../riemann-integrable-function.md) with [Riemann integral](../../../../../../riemann-integral.md) $I$ if and only if, for every $\varepsilon>0$, some $\delta>0$ satisfies

$$
\boxed{\left|\sum(f;\mathcal P,\vec\xi)-I\right|<\varepsilon}
$$

for every [partition of an interval](../../../../../../partition-of-an-interval.md) with $\|\mathcal P\|<\delta$ and every permitted choice of tags. Equivalently, along every [sequence](../../../../../../sequence.md) of such tagged [partitions of an interval](../../../../../../partition-of-an-interval.md) with [mesh of a partition](../../../../../../mesh-of-a-partition.md) tending to zero, the [Riemann sums](../../../../../../riemann-sum.md) tend to $I$. Both the shrinking [mesh of a partition](../../../../../../mesh-of-a-partition.md) and freedom of tags are essential.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

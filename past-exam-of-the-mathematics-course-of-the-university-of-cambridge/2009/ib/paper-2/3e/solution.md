<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a [contraction mapping](../../../../../contraction-mapping.md) $T:X\to X$ on a nonempty [complete metric space](../../../../../complete-metric-space.md) has a unique [fixed point](../../../../../fixed-point.md). Here contraction means that some $0\le q<1$ satisfies $d(Tx,Ty)\le qd(x,y)$ for all $x,y$.

For a proof, choose $x_0$ and iterate $x_{r+1}=Tx_r$. Induction gives $d(x_{r+1},x_r)\le q^rd(x_1,x_0)$. For $m>n$, the triangle inequality and a [geometric series](../../../../../geometric-series.md) give

$$
d(x_m,x_n)\le\sum_{r=n}^{m-1}q^rd(x_1,x_0)\le\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus the iterates form a [Cauchy sequence](../../../../../cauchy-sequence.md), and [completeness](../../../../../completeness.md) supplies a limit $a\in X$. A [contraction mapping](../../../../../contraction-mapping.md) is continuous, so $Ta=\lim Tx_n=\lim x_{n+1}=a$. If $b$ is another [fixed point](../../../../../fixed-point.md), $d(a,b)=d(Ta,Tb)\le qd(a,b)$, forcing $d(a,b)=0$. This proves existence and uniqueness.

For the exponential problem, use $h=f\circ f$ on the complete [metric space](../../../../../metric-space.md) $\mathbb R$. Its [derivative](../../../../../derivative.md) is

$$
h'(x)=e^{-x}e^{-e^{-x}}.
$$

Putting $t=e^{-x}>0$, the function $te^{-t}$ has maximum $1/e$ at $t=1$, as its [derivative](../../../../../derivative.md) is $(1-t)e^{-t}$. By the [mean value theorem](../../../../../mean-value-theorem.md), $|h(x)-h(y)|\le e^{-1}|x-y|$, so $h$ is a [contraction mapping](../../../../../contraction-mapping.md) on all of $\mathbb R$. Let $a$ be its unique [fixed point](../../../../../fixed-point.md). The compositions commute, so $h(f(a))=f(h(a))=f(a)$; uniqueness of the [fixed point](../../../../../fixed-point.md) of $h$ forces $f(a)=a$. Conversely every [fixed point](../../../../../fixed-point.md) of $f$ is fixed by $h$. Hence **there is exactly one real solution of $x=e^{-x}$**. It lies in $(0,1)$ because $a=e^{-a}>0$ and then $e^{-a}<1$. This uses the [iterated contraction](../../../../../iterated-contraction.md) argument without claiming that $f$ itself contracts on all of $\mathbb R$.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

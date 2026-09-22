<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $x>0$, the event $M_n/n\leq x$ says that each of the [independent random variables](../../../../../independent-random-variables.md) is at most $\lfloor nx\rfloor$. Hence, for all sufficiently large $n$,

$$
\mathbb P(M_n/n\leq x)=\left(1-\frac1{\lfloor nx\rfloor+1}\right)^n.
$$

Since $n/(\lfloor nx\rfloor+1)\to1/x$ and $\log(1-u)=-u+o(u)$ as $u\to0$, taking [logarithms](../../../../../logarithm.md) gives the [limit](../../../../../limit-of-a-function.md) $e^{-1/x}$. For $x\leq0$ the [probability](../../../../../probability.md) is zero. Therefore

$$
\boxed{\frac{M_n}{n}\xrightarrow{d}W,\qquad F_W(x)=\begin{cases}0,&x\leq0,\\ e^{-1/x},&x>0.\end{cases}}
$$

This is the [Fréchet limit for a reciprocal integer tail](../../../../../frechet-limit-for-a-reciprocal-integer-tail.md), with a [Fréchet distribution](../../../../../frechet-distribution.md) of shape one. Its [cumulative distribution function](../../../../../cumulative-distribution-function.md) is continuous even at zero, so the pointwise calculation establishes [convergence in distribution](../../../../../convergence-in-distribution.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

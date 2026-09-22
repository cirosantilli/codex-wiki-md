<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For an [Inhomogeneous Poisson process](../../../../../../inhomogeneous-poisson-process.md), the [likelihood function](../../../../../../likelihood-function.md) is the product of the intensities at arrivals times the exponential of minus the integrated intensity. The integrated intensity is $\theta+2(T-\theta)=2T-\theta$. There are $j(\theta)$ arrivals at rate one and $n-j(\theta)$ at rate two, so

$$
\boxed{L(\theta)=e^{\theta-2T}2^{n-j(\theta)}\ \propto\ e^\theta2^{-j(\theta)},\qquad 0<\theta<T.}
$$

Set $t_0=0$ and $t_{n+1}=T$ to include changes before the first or after the last arrival. An arrival exactly at the change has probability zero, so the convention for $j$ at that point does not affect the [Bayesian posterior](../../../../../../bayesian-posterior.md).

## ↑ Ancestors (11)

1. [G](../g.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

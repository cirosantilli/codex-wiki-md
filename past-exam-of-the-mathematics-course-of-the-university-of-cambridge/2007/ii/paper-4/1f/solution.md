<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Let $p_1,\ldots,p_a$ be the [primes](../../../../../prime-number.md) not exceeding $\sqrt x$, where $a=\pi(\sqrt x)$, and let $\Phi(x,a)$ count integers $1\leq n\leq x$ divisible by none of these primes. Every surviving integer other than $1$ is prime: a composite integer at most $x$ has a prime factor at most its square root. Conversely, the surviving primes are exactly those between $\sqrt x$ and $x$. Thus the [Legendre prime-counting formula](../../../../../legendre-prime-counting-formula.md) is

$$
\boxed{\pi(x)=\Phi(x,\pi(\sqrt x))+\pi(\sqrt x)-1\quad(x\geq1).}
$$

By [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md),

$$
\Phi(x,a)=\sum_{S\subseteq\{1,\ldots,a\}}(-1)^{|S|}
\left\lfloor\frac{x}{\prod_{i\in S}p_i}\right\rfloor,
$$

where the empty product is one. To cover literally every positive real $x$, replace the subtraction of $1$ by $\mathbf1_{\{x\geq1\}}$: for $0<x<1$, both counts are zero and there is no surviving integer $1$.

For $x=48$, the sieving primes are $2,3,5$. The surviving count is $48-(24+16+9)+(8+4+3)-1=13$. Consequently

$$
\boxed{\pi(48)=13+3-1=15.}
$$

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

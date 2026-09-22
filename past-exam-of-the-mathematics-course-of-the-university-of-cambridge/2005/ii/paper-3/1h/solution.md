<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

Let $p_1,\ldots,p_a$ be the first $a$ [primes](../../../../../prime-number.md), and let $\phi(x,a)$ count positive integers at most $x$ not divisible by any of them. The [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) gives

$$
\phi(x,a)=\sum_{S\subseteq\{1,\ldots,a\}}(-1)^{|S|}\left\lfloor\frac{x}{\prod_{j\in S}p_j}\right\rfloor.
$$

For $a=\pi(\sqrt x)$, every composite at most $x$ is removed, so the survivors are one and the [primes](../../../../../prime-number.md) larger than $\sqrt x$. Thus the [Legendre prime-counting formula](../../../../../legendre-prime-counting-formula.md) is $\boxed{\pi(x)=\phi(x,\pi(\sqrt x))+\pi(\sqrt x)-1}$. This is the prime-counting formula, distinct from the factorial-valuation formula of the same name.

Fix $y\geq2$ and put $a=\pi(y)$. Every [prime](../../../../../prime-number.md) exceeding $y$ is among the unsieved integers. Replacing each floor in the finite sum by its argument makes an error bounded by $2^a$, giving

$$
\pi(x)\leq a+\phi(x,a)\leq a+x\prod_{p\leq y}(1-1/p)+2^a.
$$

Take $x\to\infty$ with $y$ fixed. The supplied product estimate gives $0\leq\limsup\pi(x)/x\leq1/\log y$. Since $y$ can be arbitrarily large, $\boxed{\lim_{x\to\infty}\pi(x)/x=0}$. The order of these limits avoids treating the growing inclusion-exclusion error as negligible.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

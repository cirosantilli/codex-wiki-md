<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
F(n)=\prod_{i=1}^r(n+h_i)
$$

and let $W$ be the product of the finitely many primes at most $r$ or dividing some nonzero difference $h_i-h_j$. Sieve with the primes $p\nmid W$. For such a prime, the congruence $F(n)\equiv0\pmod p$ has exactly $r$ distinct roots. By the [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md), the root-counting function $\rho(d)$ is multiplicative on squarefree $d$ coprime to $W$, and

$$
\#\{n\leq x:d\mid F(n)\}
=x\frac{\rho(d)}d+O(\rho(d)).
$$

Thus the [polynomial root density in a sieve](../../../../../../polynomial-root-density-in-a-sieve.md) applies with

$$
g(p)=\frac rp,\qquad r_d=O(\rho(d)).
$$

Take $z=x^{1/4}$ and $D=z$. For squarefree $d$ coprime to $W$,

$$
h(d)=\prod_{p\mid d}\frac r{p-r}
\geq\frac{r^{\omega(d)}}d.
$$

The supplied mean-value estimate, [partial summation](../../../../../../abel-s-summation-formula.md), and removal of square factors using $r^{\omega(n)}\ll_{r,\epsilon}n^\epsilon$ give

$$
G(z,z)\gg_{r,W}(\log z)^r.
$$

The error in the [Selberg upper-bound sieve](../../../../../../selberg-upper-bound-sieve.md) is

$$
\ll\sum_{d<z^2}(3r)^{\omega(d)}
\ll_{r,\epsilon}z^{2+\epsilon}
=o\left(\frac{x}{(\log x)^r}\right).
$$

Consequently

$$
S(\mathcal A,\mathcal P;z)
\ll_{h_1,\ldots,h_r,r}\frac{x}{(\log x)^r}.
$$

If every $n+h_i$ is prime and all of them exceed $z$, then $F(n)$ has no prime divisor $p<z$ with $p\nmid W$, apart from a fixed finite set of divisibility cases absorbed into the implied constant. The cases with some $n+h_i\leq z$ contribute $O_r(z)$. Therefore

$$
\boxed{
\#\{n\leq x:n+h_1,\ldots,n+h_r\text{ are all prime}\}
\ll_{h_1,\ldots,h_r,r}\frac{x}{(\log x)^r}.
}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

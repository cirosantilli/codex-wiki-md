<h1 id="c/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Wilson's theorem](../../../../wilson-s-theorem.md) states that an integer $n>1$ is prime if and only if $(n-1)!\equiv-1\pmod n$. For a prime $p$, every nonzero residue has a [multiplicative inverse](../../../../multiplicative-inverse.md). Pair each residue with its inverse; the only self-inverse ones satisfy $(a-1)(a+1)=0$ in $\mathbb F_p$ and hence are $1,-1$ (the same residue when $p=2$). The resulting product is $-1$. Conversely, if $(n-1)!\equiv-1\pmod n$, no divisor $d$ of $n$ can satisfy $1<d<n$: it would divide both $(n-1)!$ and $n$, so could not divide $(n-1)!+1$. Hence $n$ is prime.

For a composite $n\ge6$ which is not the square of a prime, choose a proper factorization $n=ab$ with $1<a<b<n$ if possible. Both factors occur in $(n-1)!$, proving divisibility by $n$. If the initially chosen factors coincide but their common value is composite, choose a different proper divisor to obtain unequal factors; equivalently, the only composite integer all of whose proper nontrivial divisors coincide is a prime square. For $n=p^2\ge9$, the distinct factors $p$ and $2p$ lie below $p^2$ and their product is divisible by $p^2$. Thus $(n-1)!\equiv0\pmod n$ for every composite $n\ge6$.

For a prime $n$, write $(n-1)!=kn-1$. Then $\sin^2((n-1)!\pi/n)=\sin^2(\pi/n)$, so the summand is one. For a composite $n\ge6$ it is zero. The only remaining composite index is four, whose summand equals $\sin^2(3\pi/2)/\sin^2(\pi/4)=2$. Therefore the sum is the [prime-counting function](../../../../prime-counting-function.md) plus two whenever $x\ge4$; subtraction of two gives the claimed exact formula.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [C](../../c.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

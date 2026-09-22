<h1 id="1h/solution">Solution</h1>

↑ **Parent:** [1H](../1h.md)

For an odd prime $p$, the [Legendre symbol](../../../../../legendre-symbol.md) $(a/p)$ is zero if $p\mid a$, one if $a$ is a nonzero square modulo $p$, and minus one otherwise. By [Gauss lemma](../../../../../gauss-s-lemma-number-theory.md), $(2/p)=(-1)^N$, where $N$ counts those least positive residues of $2,4,\ldots,p-1$ which exceed $p/2$. They correspond to integers $j>p/4$ among $1\le j\le(p-1)/2$, hence

$$
N=\frac{p-1}{2}-\left\lfloor\frac p4\right\rfloor.
$$

For $p\equiv1,3,5,7\pmod8$, its parity is respectively $0,1,1,0$, the same as that of $(p^2-1)/8$. Therefore

$$
\boxed{\left(\frac2p\right)=(-1)^{(p^2-1)/8}.}
$$

Use multiplicativity and [quadratic reciprocity](../../../../../quadratic-reciprocity.md) for the requested composite numerator. Since $91=7\cdot13$,

$$
\left(\frac7{167}\right)=-\left(\frac{167}7\right)=-\left(\frac{-1}7\right)=1,\qquad \left(\frac{13}{167}\right)=\left(\frac{11}{13}\right)=\left(\frac2{11}\right)=-1.
$$

The first reciprocity sign is negative because both primes are $3\pmod4$; the subsequent signs are positive because one prime is $1\pmod4$. Thus **$(91/167)=-1$**.

## ↑ Ancestors (10)

1. [1H](../1h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

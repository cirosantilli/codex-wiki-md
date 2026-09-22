<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

Let $\pi$ be a [prime element](../../../../../prime-element.md) of the [Gaussian integers](../../../../../gaussian-integer.md). Its [norm](../../../../../norm.md) $\pi\overline\pi$ is a positive integer greater than one, so $\pi$ divides some ordinary positive [prime number](../../../../../prime-number.md) in its integer prime factorization. It cannot divide two distinct such primes $p,q$: an integer Bézout identity $up+vq=1$ would imply $\pi\mid1$, contrary to its being a nonunit. This proves existence and uniqueness of the rational prime lying below $\pi$.

Up to associates, the complete list of Gaussian [prime elements](../../../../../prime-element.md) is: $1+i$; the positive rational primes $p\equiv3\pmod4$; and, for every rational prime $p\equiv1\pmod4$, the two nonassociate elements $a+bi$ and $a-bi$, where $a,b>0$ and $p=a^2+b^2$. Representatives related by multiplication by one of $\pm1,\pm i$ are associates. The last pair accounts for both factors of a split prime.

Every residue class modulo $p$ has a unique representative $a+bi$ with $0\leq a,b<p$, since $p\mid(a-a')+(b-b')i$ means both coordinate differences are divisible by $p$. Hence $\boxed{|R/pR|=p^2}$ and

$$
R/pR\cong\mathbb F_p[X]/(X^2+1).
$$

For $p=2$, the class of $1+i$ is nonzero but its square is $2i=0$; thus the [quotient ring](../../../../../quotient-ring.md) is not a [field](../../../../../field.md). For $p\equiv3\pmod4$, a root $r^2=-1$ would imply $r^{p-1}=(-1)^{(p-1)/2}=-1$, contradicting [Fermat's little theorem](../../../../../fermat-little-theorem.md). The quadratic $X^2+1$ is therefore irreducible and its quotient is a [field](../../../../../field.md) with $p^2$ elements.

For $p\equiv1\pmod4$, choose a generator $g$ of the cyclic group $\mathbb F_p^\times$. Then $r=g^{(p-1)/4}$ satisfies $r^2=-1$. The two nonzero classes $i-r$ and $i+r$ have product zero in $R/pR$. Thus

$$
\boxed{R/pR\text{ is a field exactly for rational primes }p\equiv3\pmod4.}
$$

For $p\equiv1\pmod4$ it is instead isomorphic to $\mathbb F_p\times\mathbb F_p$, by the distinct linear factors and the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md).

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

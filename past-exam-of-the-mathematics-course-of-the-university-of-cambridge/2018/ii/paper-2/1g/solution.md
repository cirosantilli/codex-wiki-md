<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For an odd [prime](../../../../../prime-number.md) $p$, the [Legendre symbol](../../../../../legendre-symbol.md) is

$$
\left(\frac ap\right)=
\begin{cases}
0,&p\mid a,\\
1,&a\not\equiv0\pmod p\text{ and }a\text{ is a quadratic residue},\\
-1,&a\text{ is a quadratic nonresidue}.
\end{cases}
$$

[Gauss lemma](../../../../../gauss-s-lemma-riemannian-geometry.md) says that if $p\nmid a$ and $N$ of the least positive residues of

$$
a,2a,\ldots,\frac{p-1}{2}a
$$

exceed $p/2$, then $(a/p)=(-1)^N$.

For $a=2$, none of $2,4,\ldots,p-1$ needs reduction modulo $p$, and the terms exceeding $p/2$ are those with $j>p/4$. Hence

$$
N=\frac{p-1}{2}-\left\lfloor\frac p4\right\rfloor.
$$

Checking $p\equiv1,3,5,7\pmod8$ shows that $N$ has the same parity as $(p^2-1)/8$. Therefore

$$
\boxed{\left(\frac2p\right)=(-1)^{(p^2-1)/8}.}
$$

By [quadratic reciprocity](../../../../../quadratic-reciprocity.md), and because $149\equiv1\pmod4$,

$$
\left(\frac{105}{149}\right)
=\left(\frac3{149}\right)
 \left(\frac5{149}\right)
 \left(\frac7{149}\right)
=\left(\frac2{3}\right)
 \left(\frac4{5}\right)
 \left(\frac2{7}\right).
$$

The three factors are $-1,1,1$, respectively, so

$$
\boxed{\left(\frac{105}{149}\right)=-1.}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

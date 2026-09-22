<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

In a [principal ideal domain](../../../../../principal-ideal-domain.md), an ascending chain of [ideals](../../../../../ideal.md) stabilizes: its union is an [ideal](../../../../../ideal.md) $(d)$, and its generator belongs to one member, which then contains the union. This proves the needed [ascending chain condition](../../../../../ascending-chain-condition.md). If a nonzero nonunit had no finite irreducible factorization, split it into two nonunits and select a factor that still has no such factorization. Continuing would give a strictly ascending chain of principal [ideals](../../../../../ideal.md), because $a=bc$ with $c$ a nonunit implies $(a)\subsetneq(b)$. This contradicts the chain condition, so factorization exists.

An [irreducible element](../../../../../irreducible-element.md) $p$ generates a [maximal ideal](../../../../../maximal-ideal.md): any intermediate [ideal](../../../../../ideal.md) is $(d)$ with $p=dc$, and irreducibility forces $d$ or $c$ to be a unit. Therefore $p$ is a [prime element](../../../../../prime-element.md). In any two irreducible factorizations, the first prime factor divides a factor of the other, hence is associate to it. Cancel and continue. This proves **every [principal ideal domain](../../../../../principal-ideal-domain.md) is a [unique factorization domain](../../../../../unique-factorization-domain.md)**.

In $\mathbb Z[\sqrt{-3}]$, the multiplicative [field norm](../../../../../field-norm.md) is $N(a+b\sqrt{-3})=a^2+3b^2$. The only [units](../../../../../unit-in-a-ring.md) are $\pm1$. There is no element of norm two, so every element of norm four is irreducible: a factorization into nonunits would require norms two and two. Consequently

$$
\boxed{4=2\cdot2=(1+\sqrt{-3})(1-\sqrt{-3})}
$$

is a pair of genuinely different irreducible factorizations. Neither $1+\sqrt{-3}$ nor $1-\sqrt{-3}$ is associate to $2$.

Take the [Eisenstein integers](../../../../../eisenstein-integer.md) $R=\mathbb Z[\omega]$, where $\omega=(-1+\sqrt{-3})/2$ and $\omega^2+\omega+1=0$. Since $\sqrt{-3}=1+2\omega$, the embedded subring is $\mathbb Z+2\mathbb Z\omega$, whose additive index in $R$ is two. Its larger ring has [Eisenstein-integer norm](../../../../../eisenstein-integer-norm.md) $N(a+b\omega)=a^2-ab+b^2$ and is Euclidean. Indeed, write a complex quotient in the real basis $1,\omega$ and round both coordinates to integers. The coordinate errors $u,v$ satisfy $|u|,|v|\le1/2$, giving $|u+v\omega|^2=u^2-uv+v^2\le3/4<1$. Thus division leaves a remainder of smaller norm. A [Euclidean domain](../../../../../euclidean-domain.md) is a [principal ideal domain](../../../../../principal-ideal-domain.md), because division by a nonzero element of least norm in an ideal leaves zero remainder. This gives the requested **index-two embedding into a [principal ideal domain](../../../../../principal-ideal-domain.md)**.

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

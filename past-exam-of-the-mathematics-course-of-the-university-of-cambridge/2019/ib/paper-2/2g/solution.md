<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Let the [torsion submodule](../../../../../torsion-submodule.md) of the [module over a ring](../../../../../module-mathematics.md) $M$ be

$$
T(M)=\{m\in M:rm=0\text{ for some }0\ne r\in R\}.
$$

This is a [submodule](../../../../../submodule.md). Indeed, if $rm=0$ and $sn=0$ with $r,s\ne0$, then $rs\ne0$ because the scalar ring is an [integral domain](../../../../../integral-domain.md), and $rs(m+n)=0$; scalar multiples and additive inverses are handled similarly.

Take the [quotient module](../../../../../quotient-module.md) $M_0=M/T(M)$ and let $q:M\to M_0$ be the quotient [R-module homomorphism](../../../../../module-homomorphism.md). It is [torsion-free](../../../../../torsion-free-module.md): if $0\ne r\in R$ and $r(m+T(M))=0$, then $rm\in T(M)$, so $srm=0$ for some $s\ne0$. Since $sr\ne0$, this puts $m$ in $T(M)$ and therefore $m+T(M)=0$.

Now let $N$ be torsion-free and let $f:M\to N$ be an $R$-module homomorphism. If $m\in T(M)$ and $rm=0$ for $r\ne0$, then $r f(m)=f(rm)=0$, so torsion-freeness gives $f(m)=0$. Hence $T(M)\subseteq\ker f$, and the [universal property of a quotient module](../../../../../universal-property-of-a-quotient-module.md) gives a unique homomorphism

$$
f_0:M/T(M)\longrightarrow N,
\qquad f_0(m+T(M))=f(m),
$$

with $\boxed{f=f_0\circ q}$. Thus $M/T(M)$ is the [maximal torsion-free quotient](../../../../../maximal-torsion-free-quotient.md) of $M$.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

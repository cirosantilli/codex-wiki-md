<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

For an odd [prime number](../../../../../prime-number.md) $p$, the [Legendre symbol](../../../../../legendre-symbol.md) is zero when $p\mid a$, one when $a$ is a nonzero [quadratic residue](../../../../../quadratic-residue.md) modulo $p$, and minus one otherwise. The number-theoretic [Gauss lemma](../../../../../gauss-s-lemma-number-theory.md) says that, for $p\nmid a$, $(a/p)=(-1)^r$, where $r$ counts those least positive residues of $a,2a,\ldots,(p-1)a/2$ exceeding $p/2$.

For $a=2$, the residues are simply $2,4,\ldots,p-1$, so $r=(p-1)/2-\lfloor p/4\rfloor$. Examining the four odd residue classes modulo eight gives

$$
\boxed{\left(\frac2p\right)=(-1)^{(p^2-1)/8}
=\begin{cases}1&p\equiv1,7\pmod8,\\-1&p\equiv3,5\pmod8.\end{cases}}
$$

Now $2^m\equiv-1\pmod p$ and $p$ is odd. The [multiplicative order](../../../../../multiplicative-order.md) $d$ of $2$ divides $2m$ but not $m$. Since $m$ is a power of two, every proper divisor of $2m$ divides $m$, whence $d=2m$. [Lagrange's theorem for finite groups](../../../../../lagrange-s-theorem.md) gives $2m\mid p-1$. Because $m\ge4$, this implies $p\equiv1\pmod8$, so the supplementary law just proved gives $(2/p)=1$. By [Euler's criterion](../../../../../euler-s-criterion.md), $2^{(p-1)/2}\equiv1\pmod p$, and consequently $2m\mid(p-1)/2$. Therefore

$$
\boxed{p\equiv1\pmod{4m}}.
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work with the usual commutative unital [ring](../../../../../../ring.md) convention. Write $f(T)=a_1T+a_2T^2+\cdots$, where $a_1=f'(0)$ is a [unit](../../../../../../unit-in-a-ring.md), and seek $g(T)=\sum_{n\ge1}b_nT^n$. Since $g$ has zero constant term, every coefficient of the composition of these [formal power series](../../../../../../formal-power-series.md) involves only finitely many terms.

The linear coefficient forces $b_1=a_1^{-1}$. Suppose $b_1,\ldots,b_{n-1}$ have been chosen. The coefficient of $T^n$ in $f(g(T))$ is

$$
a_1b_n+C_n(a_2,\ldots,a_n;b_1,\ldots,b_{n-1}).
$$

Indeed the term involving $b_n$ can only come from $a_1g$: in $g^j$ with $j\ge2$, using a degree-$n$ term forces total degree at least $n+j-1>n$. Choose $b_n=-a_1^{-1}C_n$. This [recursive construction of a compositional inverse](../../../../../../recursive-construction-of-a-compositional-inverse.md) uniquely gives $f\circ g=T$.

To check the other composition rather than assume it, construct $h(T)=\sum_{n\ge1}c_nT^n$ satisfying $h\circ f=T$. At degree $n$, its new coefficient is $c_na_1^n$ plus terms already determined; $a_1^n$ is a [unit](../../../../../../unit-in-a-ring.md), so the same recursion works. Composition is associative, as can be checked coefficientwise, or after truncation modulo $T^{N+1}$ for every $N$. Therefore

$$
h=h\circ(f\circ g)=(h\circ f)\circ g=g.
$$

Consequently the [compositional inverse of a formal power series](../../../../../../compositional-inverse-of-a-formal-power-series.md) is unique and satisfies

$$
\boxed{f(g(T))=g(f(T))=T.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

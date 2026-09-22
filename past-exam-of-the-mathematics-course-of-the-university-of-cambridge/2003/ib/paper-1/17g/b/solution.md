<h1 id="17g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply [Euler's criterion](../../../../../../euler-s-criterion.md) to $-1$. It gives

$$
\boxed{\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2}=\begin{cases}1,&p\equiv1\pmod4,\\-1,&p\equiv3\pmod4.\end{cases}}
$$

For $p\nmid ab$, the same criterion gives $(ab/p)\equiv (ab)^{(p-1)/2}=a^{(p-1)/2}b^{(p-1)/2}\equiv(a/p)(b/p)\pmod p$. Both sides are integers in $\{1,-1\}$, which are distinct modulo an odd prime, so congruence implies equality. This proves [multiplicativity of the Legendre symbol](../../../../../../multiplicativity-of-the-legendre-symbol.md):

$$
\boxed{\left(\frac{ab}{p}\right)=\left(\frac ap\right)\left(\frac bp\right).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17G](../../17g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

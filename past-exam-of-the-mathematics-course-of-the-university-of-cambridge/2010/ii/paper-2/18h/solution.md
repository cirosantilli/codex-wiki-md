<h1 id="18h/solution">Solution</h1>

↑ **Parent:** [18H](../18h.md)

For the first field, set $K=\mathbb Q(\sqrt5,i)$. Its [field extension degree](../../../../../degree-of-a-field-extension.md) is four, since $\mathbb Q(\sqrt5)$ is real and adjoining $i$ doubles its degree. The [polynomial](../../../../../polynomial-split.md) $X^3-5$ is irreducible over $K$: a reducible cubic would have a root in $K$, but every root has degree three over $\mathbb Q$ by [Eisenstein criterion](../../../../../eisenstein-criterion.md), impossible by the [tower law](../../../../../tower-law.md) because $3\nmid4$. Thus

$$
\boxed{[\mathbb Q(\sqrt[3]5,\sqrt5,i):\mathbb Q]=12}.
$$

For the second field, put $\alpha=\sqrt[4]5>0$. The [splitting field](../../../../../splitting-field.md) is $F=\mathbb Q(\alpha,i)$ and has degree eight, since $X^4-5$ is Eisenstein and $\mathbb Q(\alpha)$ is real. Define [automorphisms](../../../../../automorphism.md) $r(\alpha)=i\alpha,r(i)=i$ and $s(\alpha)=\alpha,s(i)=-i$. They satisfy $r^4=s^2=1$ and $srs=r^{-1}$, and give eight distinct automorphisms. Hence **$\operatorname{Gal}(F/\mathbb Q)\cong D_8$.**

The [Galois correspondence](../../../../../galois-correspondence.md) gives all the subfields in the following table. The middle column records generators, not merely their degrees.

$$
\begin{array}{c|c|c}
\text{subgroup fixing the field}&\text{field}&\text{degree over }\mathbb Q\\ \hline
\langle r,s\rangle&\mathbb Q&1\\
\langle r\rangle&\mathbb Q(i)&2\\
\langle r^2,s\rangle&\mathbb Q(\sqrt5)&2\\
\langle r^2,rs\rangle&\mathbb Q(i\sqrt5)&2\\
\langle r^2\rangle&\mathbb Q(\sqrt5,i)&4\\
\langle s\rangle&\mathbb Q(\alpha)&4\\
\langle r^2s\rangle&\mathbb Q(i\alpha)&4\\
\langle rs\rangle&\mathbb Q((1+i)\alpha)&4\\
\langle r^3s\rangle&\mathbb Q((1-i)\alpha)&4\\
\{1\}&F&8
\end{array}
$$

Each displayed generator is fixed by the indicated subgroup. The two last quartic generators have fourth power $-20$, so their degree is four by [Eisenstein criterion](../../../../../eisenstein-criterion.md); the other quartic degrees are immediate. These are all the subgroups of $D_8$ and hence all the subextensions.

## ↑ Ancestors (10)

1. [18H](../18h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

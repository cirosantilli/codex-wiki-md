<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For odd $p$, eighth roots of unity have order prime to the residue characteristic. The [total ramification criterion for local cyclotomic extensions](../../../../../../total-ramification-criterion-for-local-cyclotomic-extensions.md) shows that they generate an unramified extension of degree $f=\operatorname{ord}_8(p)$. More directly, a primitive eighth root in $\mathbb F_{p^f}$ lifts uniquely by [Hensel lemma](../../../../../../hensel-s-lemma.md), since the derivative of $T^8-1$ is a unit at each nonzero root. Its residue has exact order eight, and the [Frobenius automorphism](../../../../../../frobenius-automorphism.md) acts by $\zeta_8\mapsto\zeta_8^p$. Consequently $f=1$ when $p\equiv1\pmod8$ and $f=2$ for the other three odd residue classes.

At $p=2$, the translated [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) is

$$
\Phi_8(1+T)=(1+T)^4+1=T^4+4T^3+6T^2+4T+2.
$$

It is [Eisenstein](../../../../../../eisenstein-criterion.md) at two, so the extension has degree four. All primitive eighth roots are odd powers of $\zeta_8$ and already lie in the field; the extension is Galois, and its automorphisms give the full group $(\mathbb Z/8\mathbb Z)^\times\cong C_2\times C_2$. Thus

$$
\boxed{\operatorname{Gal}(\mathbb Q_p(\zeta_8)/\mathbb Q_p)\cong
\begin{cases}C_2\times C_2,&p=2,\\1,&p\equiv1\pmod8,\\C_2,&p\equiv3,5,7\pmod8.\end{cases}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

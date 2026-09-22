<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $L_\tau=\mathbb Z\tau+\mathbb Z$, the index-$p$ overlattices are

$$
L_b=\mathbb Z\frac{\tau+b}{p}+\mathbb Z\quad(0\le b<p),\qquad L_\infty=\mathbb Z\tau+\frac1p\mathbb Z.
$$

The first $p$ preserve the marked point $1/N$. At a good prime the last equals $p^{-1}L_{p\tau}$, with marked point corresponding after scaling to $p/N$. Consequently the lattice formula becomes

$$
\boxed{T_pf(\tau)=\frac1p\sum_{b=0}^{p-1}f\left(\frac{\tau+b}{p}\right)+p^{k-1}\chi(p)f(p\tau)\quad(p\nmid N).}
$$

The first term has coefficient $a_{pn}$, because the sum of $p$th [roots of unity](../../../../../../root-of-unity.md) is zero unless its exponent is divisible by $p$. The second has coefficient $\chi(p)p^{k-1}a_{n/p}$ when $p\mid n$ and zero otherwise. Thus

$$
\boxed{b_n=\begin{cases}a_{pn},&p\nmid n,\\a_{pn}+\chi(p)p^{k-1}a_{n/p},&p\mid n.\end{cases}}
$$

This includes $b_0=(1+\chi(p)p^{k-1})a_0$ at a good prime.

At $p\mid N$, the last overlattice loses the required exact order and is excluded. The operator is then $U_p$, with $b_n=a_{pn}$. The formula remains valid for all primes if the [Dirichlet character](../../../../../../dirichlet-character.md) is extended to integers by zero on nonunits, so $\chi(p)=0$ at bad primes. Without that extension, the printed $\chi(p)$ is defined only when $p\nmid N$. This is the [good-prime and bad-prime Hecke coefficient formula](../../../../../../good-prime-and-bad-prime-hecke-coefficient-formula.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

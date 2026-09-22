<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $a,b\in H^2(S^2\times S^2;\mathbb Z)$ be the two factor classes, normalized by $a^2=b^2=0$ and $\langle ab,[X]\rangle=1$. Choose the [complex line bundle](../../../../../../complex-line-bundle.md) $L$ with $c_1(L)=a+b$, for example the tensor product of pullbacks of degree-one [complex line bundles](../../../../../../complex-line-bundle.md) from the two factors. Then

$$
c_1(L)^2[X]=2.
$$

If $L$ had an [ASD connection](../../../../../../anti-self-dual-connection.md), the real closed form $\alpha=iF/(2\pi)$ would represent this class and satisfy $*\alpha=-\alpha$. Hence

$$
2=\int_X\alpha\wedge\alpha=-\int_X|\alpha|^2\,d\mathrm{vol}_g\leq0,
$$

a contradiction. **This [complex line bundle](../../../../../../complex-line-bundle.md) admits no ASD connection for any metric of the given product orientation.** For the reverse product orientation, take $c_1(L)=a-b$ instead, which then has square $+2$. This is the [positive-square obstruction to ASD line connections](../../../../../../positive-square-obstruction-to-asd-line-connections.md).

The suggested rank-two construction gives the same obstruction. The split bundle $E=L\oplus L^*$ has trivial determinant and

$$
c(E)=(1+c_1(L))(1-c_1(L)),\qquad c_2(E)[X]=-c_1(L)^2[X]=-2.
$$

An [ASD connection](../../../../../../anti-self-dual-connection.md) on $L$ would induce an [ASD connection](../../../../../../anti-self-dual-connection.md) on $E$, but its [instanton number](../../../../../../instanton-number.md) would be $\|F_E\|_2^2/(8\pi^2)\geq0$, contradicting $c_2(E)[X]=-2$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

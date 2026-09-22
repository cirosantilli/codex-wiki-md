<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [morphism of schemes](../../../../../../morphism-of-schemes.md) $f:X\to Y$ is a [flat morphism](../../../../../../flat-morphism.md) when every local-ring map $\mathcal O_{Y,f(x)}\to\mathcal O_{X,x}$ makes $\mathcal O_{X,x}$ a [flat module](../../../../../../flat-module.md).

In (i), the coordinate map is $k[t]\to k[y]$, $t\mapsto y^2$, and

$$
k[y]=k[t]\oplus yk[t].
$$

It is therefore a [free module](../../../../../../free-module.md) of rank two and the morphism is flat, including in characteristic two.

In (ii), $k[x]$ is finite over the cusp ring $R=k[x^2,x^3]$ and has generic rank one. Were it flat, finite flatness over the local ring at the cusp would make it free of rank one. Its fiber there is instead

$$
k[x]\otimes_R R/(x^2,x^3)\simeq k[x]/(x^2),
$$

which has dimension two, so this morphism is not flat.

In (iii), the base coordinate $t$ acts as $x$, and the nonzero element $y$ satisfies $ty=xy=0$. Thus the coordinate ring has torsion as a $k[t]$-module. Since $k[t]$ is a [principal ideal domain](../../../../../../principal-ideal-domain.md) and a module over it is flat exactly when it is torsion-free, this morphism is not flat. Consequently

$$
\boxed{\text{only (i) is flat}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A positive integer $D$ is a [congruent number](../../../../../../congruent-number.md) when it is the area of a right triangle with positive rational side lengths. For a point $P=(x,y)$ with $y\ne0$ on

$$
E_D:y^2=x^3-D^2x,
$$

the formulas

$$
a=\frac{x^2-D^2}{y},
\qquad b=\frac{2Dx}{y},
\qquad c=\frac{x^2+D^2}{y}
$$

give $a^2+b^2=c^2$ and $ab/2=D$, after changing signs if necessary. Conversely, a rational right triangle of area $D$ gives

$$
x=\frac{D(a+c)}b,
\qquad y=\frac{2D^2(a+c)}{b^2},
$$

so these constructions are inverse up to the usual sign choices.

It remains to distinguish torsion. If an odd prime $\ell$ divided the order of a rational torsion point, choose by the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) a good prime $p\equiv3\pmod4$ for which $p\not\equiv-1\pmod\ell$. Part (a) gives $\#E_D(\mathbb F_p)=p+1$, while part (b), applied to the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md), makes reduction injective on $\ell$-power torsion because $\ell$ is a unit in $\mathbb Z_p$. This is impossible. Similarly, a good prime $p\equiv3\pmod8$ shows that the rational $2$-primary torsion has order at most four. Since

$$
O,(0,0),(D,0),(-D,0)
$$

already form the full rational [2-torsion](../../../../../../2-torsion.md),

$$
E_D(\mathbb Q)_{\mathrm{tors}}\cong(\mathbb Z/2\mathbb Z)^2.
$$

The triangle construction uses exactly the points with $y\ne0$, which are therefore nontorsion. By the [Mordell-Weil theorem](../../../../../../mordell-weil-group.md), such a point exists exactly when the free part has positive rank. Hence

$$
\boxed{D\text{ is congruent}\quad\Longleftrightarrow\quad\operatorname{rank}E_D(\mathbb Q)\geq1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

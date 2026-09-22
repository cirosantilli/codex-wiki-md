<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A=k[x,y]$ and $\mathfrak m=(x,y)$. Since $f(0,0)\ne0$, the [principal open subscheme](../../../../../../principal-open-subscheme.md) $D(f)=\operatorname{Spec}A_f$ contains $\mathfrak m$, and

$$
V=D(f)\setminus\{\mathfrak m\}.
$$

Cover $V$ by the two affine opens $D(xf)$ and $D(yf)$, whose intersection is $D(xyf)$. The degree-zero part of the resulting [Čech cohomology](../../../../../../cech-cohomology.md) complex gives

$$
H^0(V,\mathcal O_V)=A_{xf}\cap A_{yf}=A_f
$$

inside the [fraction field](../../../../../../field-of-fractions.md) of $A$. The last equality follows because $A_f$ is a [unique factorization domain](../../../../../../unique-factorization-domain.md) and a rational function regular after localizing at both $x$ and $y$ has no possible prime factor left in its denominator.

The same affine cover is acyclic, so its degree-one Čech group computes [sheaf cohomology](../../../../../../sheaf-cohomology.md) and gives

$$
H^1(V,\mathcal O_V)
\cong A_{xyf}/(A_{xf}+A_{yf}).
$$

Before localizing at $f$, the quotient

$$
Q=A_{xy}/(A_x+A_y)
$$

has the $k$-basis

$$
\{x^{-a}y^{-b}:a,b\geq1\}.
$$

Writing $f=c+h$ with $c=f(0,0)\in k^\times$ and $h\in(x,y)$, multiplication by $h$ is locally nilpotent on $Q$: for each negative monomial, a sufficiently high power of $(x,y)$ moves every term into $A_x+A_y$. Hence $c+h$ acts invertibly on $Q$ by a finite geometric series on each element. Localizing at $f$ therefore leaves $Q$ unchanged, and

$$
H^1(V,\mathcal O_V)\cong Q_f\cong Q.
$$

The displayed infinite basis proves that this vector space is infinite-dimensional.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

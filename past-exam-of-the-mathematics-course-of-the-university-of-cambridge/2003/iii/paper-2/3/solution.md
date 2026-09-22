<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [regular element of a ring](../../../../../regular-element-of-a-ring.md) is an element $c$ for which both multiplication maps are injective:

$$
cr=0\Longrightarrow r=0,\qquad rc=0\Longrightarrow r=0.
$$

It is thus neither a left nor a right zero divisor; it need not be a unit. Here “ideals” means two-sided ideals. Put $A=A_n(\mathbb C)$, and let $T_2(A)$ denote the specified upper triangular ring.

We first establish the additional facts about the [Weyl algebra](../../../../../weyl-algebra.md) needed below. Its generators satisfy

$$
[x_i,x_j]=[\partial_i,\partial_j]=0,\qquad [\partial_i,x_j]=\delta_{ij}.
$$

Reordering gives a spanning set $x^\alpha\partial^\beta$. These monomials are independent. Indeed, represent the generators by multiplication and differentiation on $\mathbb C[x_1,\ldots,x_n]$. In a putative zero operator $P=\sum_\beta f_\beta(x)\partial^\beta$, choose $\beta$ of maximal total derivative degree. Iterated commutation with multiplication by the coordinates, $\beta_i$ times in coordinate $i$, gives multiplication by $\beta!f_\beta(x)$. All other derivative terms of that total degree disappear unless they have exactly the same multiindex, and lower-degree terms disappear. Thus $f_\beta=0$, and descending induction eliminates all coefficients. This proves the [ordered monomial basis of a Weyl algebra](../../../../../ordered-monomial-basis-of-a-weyl-algebra.md) and faithfulness of its polynomial action.

The [Weyl algebra](../../../../../weyl-algebra.md) is a [simple ring](../../../../../simple-ring.md). In a nonzero two-sided ideal choose a nonzero element of least [Bernstein filtration](../../../../../bernstein-filtration.md) degree, where both $x_i$ and $\partial_i$ have degree one. Commuting it with any generator stays in the ideal and lowers that degree. Minimality therefore makes all these commutators zero. Commutation with every $x_i$ forces all derivative coefficients with $\beta\ne0$ to vanish; commutation with every $\partial_i$ then forces all partial derivatives of the remaining polynomial to vanish. In characteristic zero the element is a nonzero scalar. The ideal consequently contains $1$. This proves [simplicity of a Weyl algebra in characteristic zero](../../../../../simplicity-of-a-weyl-algebra-in-characteristic-zero.md). Its [Jacobson radical](../../../../../jacobson-radical.md) is zero, since the radical is a proper two-sided ideal of a nonzero unital simple ring.

Use the two diagonal idempotents to isolate the entries of any ideal of $T_2(A)$. It must have the form

$$
\begin{pmatrix}I_{11}&I_{12}\\0&I_{22}\end{pmatrix},
$$

where all three entries are two-sided ideals of $A$ and $I_{11}A+AI_{22}\subseteq I_{12}$. Conversely this condition makes the indicated set an ideal. Simplicity says that each $I_{ij}$ is $0$ or $A$, and either nonzero diagonal entry forces $I_{12}=A$. Hence **the five ideals of $R_1$ are**

$$
\boxed{0,\quad
N=\begin{pmatrix}0&A\\0&0\end{pmatrix},\quad
\begin{pmatrix}A&A\\0&0\end{pmatrix},\quad
\begin{pmatrix}0&A\\0&A\end{pmatrix},\quad R_1.}
$$

For a two-sided ideal of $M_2(A)$, multiplication on both sides by elementary matrices isolates any entry and moves it to any matrix position. The entries obtained form one two-sided ideal $I$ of $A$, and the original ideal is $M_2(I)$. Thus **the only ideals of $R_2$ are $0$ and $R_2$**.

Since $N^2=0$, $N$ lies in the [Jacobson radical](../../../../../jacobson-radical.md) of $R_1$: for $z\in N$ and $r\in R_1$, $zr\in N$ and $1-zr$ has inverse $1+zr$. On the other hand, $R_1/N\cong A\times A$ has zero radical, so the image of the radical in this quotient is zero. The elementary [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md) justifies both assertions. Therefore

$$
\boxed{J(R_1)=N,\qquad J(R_2)=0.}
$$

The second equality follows from simplicity of $R_2$.

We now construct the denominators used to describe regular matrices. A left [Noetherian](../../../../../noetherian-ring.md) [noncommutative domain](../../../../../noncommutative-domain.md) satisfies the left [Ore condition](../../../../../ore-condition.md). For if $Aa\cap Ab=0$ for two nonzero elements, the left ideals $Ab, Aba, Aba^2,\ldots$ have direct sum: in a relation the first summand lies in $Ab$, all the others in $Aa$, so it vanishes; cancellation of the final $a$ repeats the argument. Their finite partial sums form a strictly ascending chain, contradicting left Noetherianity. Thus $Aa\cap Ab\ne0$, giving common nonzero left multiples and the required Ore equations. The analogous argument with right ideals gives the right [Ore condition](../../../../../ore-condition.md) under right Noetherianity. Both hypotheses for $A$ are allowed in the question.

The [Ore localization](../../../../../ore-localization.md) therefore embeds $A$ in a [division ring](../../../../../division-ring.md) $Q$. Briefly, its elements are left fractions $a^{-1}b$, with nonzero $a$, and two fractions are identified after passing to a common left denominator. Common multiples supply addition and multiplication, while cancellation in the domain makes the embedding injective. A nonzero fraction has an inverse, obtained by interchanging its numerator and denominator in the appropriate Ore fraction calculation. The right fraction construction gives the same division ring, so finite lists have common left and common right denominators.

A triangular matrix $c=\begin{pmatrix}r&s\\0&t\end{pmatrix}$ with $r,t\ne0$ is invertible over $T_2(Q)$, with inverse

$$
\begin{pmatrix}r^{-1}&-r^{-1}st^{-1}\\0&t^{-1}\end{pmatrix}.
$$

It is consequently regular over $T_2(A)$. If $r=0$, then $cE_{11}=0$; if $t=0$, then $E_{22}c=0$. Hence

$$
\boxed{\operatorname{Reg}(R_1)=
\left\{\begin{pmatrix}r&s\\0&t\end{pmatrix}:r,t\ne0\right\}.}
$$

A full matrix is regular exactly when it is invertible over $Q$:

$$
\boxed{\operatorname{Reg}(R_2)=M_2(A)\cap\operatorname{GL}_2(Q).}
$$

One implication follows immediately from invertibility. Conversely, a singular matrix over a [division ring](../../../../../division-ring.md) has a nonzero right kernel column and a nonzero left kernel row, by row reduction. A common right denominator turns the column into a nonzero column over $A$, providing a right annihilator matrix over $A$. A common left denominator does the same for the row and gives a left annihilator. Thus a singular matrix is not regular. Explicitly, for $c=\begin{pmatrix}r&s\\t&u\end{pmatrix}$ with $r\ne0$, row elimination says that regularity is equivalent to $u-tr^{-1}s\ne0$ in $Q$. If $r=0$, it is equivalent to both $s\ne0$ and $t\ne0$. A commutative determinant formula must not be substituted here.

Finally both [classical left rings of quotients](../../../../../classical-left-ring-of-quotients.md) exist, and

$$
\boxed{Q^l_{\mathrm{cl}}(R_1)=T_2(Q),\qquad
Q^l_{\mathrm{cl}}(R_2)=M_2(Q).}
$$

To prove this directly, clear a common left denominator $a\ne0$ from all the finitely many entries of a matrix over $Q$. It becomes $(aI_2)^{-1}b$ with $b$ in the original triangular or full ring and $aI_2$ regular. Every original regular element becomes a unit in the corresponding ring over $Q$, by the descriptions above. For $c$ regular and $r$ in the original ring, write $rc^{-1}=d^{-1}b$ in this way; then $dr=bc$, the left [Ore condition](../../../../../ore-condition.md). Since the denominators are regular, the additional annihilator condition for localization is automatic. This proves the [matrix and triangular localization over an Ore domain](../../../../../matrix-and-triangular-localization-over-an-ore-domain.md) assertions. In particular, the nonzero nilpotent radical of the triangular ring does not prevent its classical localization; that localization retains the triangular radical.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

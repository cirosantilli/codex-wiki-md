<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [quantum plane](../../../../../../quantum-plane.md) $A=k\langle x,y\rangle/(yx-qxy)$ and the [quantum enveloping algebra of sl2](../../../../../../quantum-enveloping-algebra-of-sl2.md) [comultiplication](../../../../../../comultiplication.md) from Question 2. The generator actions are $Kx=qx$, $Ky=q^{-1}y$, $Ex=0$, $Ey=x$, $Fx=y$, $Fy=0$. Extend them by the [module algebra](../../../../../../module-algebra.md) rules

$$
E(ab)=(Ea)(Kb)+a(Eb),\qquad
F(ab)=(Fa)b+(K^{-1}a)(Fb),\qquad K(ab)=(Ka)(Kb).
$$

These descend to $A$: $E(yx)=qx^2=E(qxy)$ and $F(yx)=qy^2=F(qxy)$, while $K$ preserves $yx-qxy$. For the ordered [monomial basis](../../../../../../monomial-basis.md), induction with $[s+1]=q^{-1}[s]+q^s$ gives the [quantum enveloping algebra action on the quantum plane](../../../../../../quantum-enveloping-algebra-action-on-the-quantum-plane.md)

$$
\boxed{K(x^ry^s)=q^{r-s}x^ry^s,\quad
E(x^ry^s)=[s]x^{r+1}y^{s-1},\quad
F(x^ry^s)=[r]x^{r-1}y^{s+1}.}
$$

Terms with a negative exponent have zero coefficients and are interpreted as zero.

We now verify the defining relations explicitly on every [basis](../../../../../../basis.md) vector, rather than infer them merely from the generator actions. The $K$ [weight](../../../../../../weight-representation-theory.md) changes by $q^2$ under $E$ and $q^{-2}$ under $F$, so $KE=q^2EK$ and $KF=q^{-2}FK$. Also

$$
\begin{aligned}
(EF-FE)(x^ry^s)
&=\bigl([r][s+1]-[s][r+1]\bigr)x^ry^s\\
&=[r-s]x^ry^s
=\frac{K-K^{-1}}{q-q^{-1}}(x^ry^s).
\end{aligned}
$$

The middle identity follows by inserting $[j]=(q^j-q^{-j})/(q-q^{-1})$ and cancelling the terms $q^{r+s+1}$ and $q^{-r-s-1}$; the remaining numerator is $(q-q^{-1})(q^{r-s}-q^{s-r})$. Finally $KK^{-1}=1$. Thus all the rank-one defining relations hold. The phrase “Serre relations” here refers to these rank-one presentation relations; there are no additional relations involving distinct simple roots for $\mathfrak{sl}_2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="32d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D=[A,B]$, so $[A,D]=[B,D]=0$. Repeated use of the product rule for the [commutator](../../../../../../commutator.md) gives $[A,B^n]=nDB^{n-1}$. Summing the exponential series yields

$$
\boxed{[A,e^B]=De^B.}
$$

These manipulations hold for [bounded operators](../../../../../../continuous-linear-operator.md), or as identities on a common invariant domain where the series and derivatives are justified.

The same commutation relation implies $e^{\lambda A}Be^{-\lambda A}=B+\lambda D$: its derivative is $e^{\lambda A}[A,B]e^{-\lambda A}=D$ and its initial value is $B$. Put $G(\lambda)=e^{\lambda A}e^{\lambda B}$. Then

$$
G'=(A+B+\lambda D)G.
$$

For the specified $F(\lambda)=G(\lambda)e^{-\lambda(A+B)}$, the operator $G$ commutes with $A+B$. Indeed conjugation by $e^{\lambda B}$ sends $A+B$ to $A+B-\lambda D$, and subsequent conjugation by $e^{\lambda A}$ restores $A+B$. Therefore

$$
F'=(A+B+\lambda D)F-F(A+B)=\lambda DF,\qquad F(0)=I,
$$

so $F(\lambda)=e^{\lambda^2D/2}$. At $\lambda=1$ this proves the central-commutator case of the [Baker--Campbell--Hausdorff formula](../../../../../../baker-campbell-hausdorff-formula.md):

$$
\boxed{e^Ae^B=e^{[A,B]/2}e^{A+B}=e^{A+B}e^{[A,B]/2}.}
$$

The last equality holds because $D$ commutes with $A+B$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [32D](../../32d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because the direction of a [lax monoidal functor](../../../../../../monoidal-functor.md) compares the target tensor with the image of the source tensor, the given maps $\varphi_{X,Y}:X\bullet Y\to X\diamond Y$ have the correct direction. They need not be invertible unless a [strong monoidal functor](../../../../../../strong-monoidal-functor.md) is intended.

Their associativity condition is the following [commutative diagram](../../../../../../commutative-diagram.md), with the [associators](../../../../../../associator.md) of the two structures labelled explicitly:

$$
\begin{array}{ccccc}
(X\bullet Y)\bullet Z&\xrightarrow{\varphi_{X,Y}\bullet1}&(X\diamond Y)\bullet Z&\xrightarrow{\varphi_{X\diamond Y,Z}}&(X\diamond Y)\diamond Z\\
\alpha^\bullet\downarrow&&&&\downarrow\alpha^\diamond\\
X\bullet(Y\bullet Z)&\xrightarrow{1\bullet\varphi_{Y,Z}}&X\bullet(Y\diamond Z)&\xrightarrow{\varphi_{X,Y\diamond Z}}&X\diamond(Y\diamond Z).
\end{array}
$$

The two unit conditions, since $\varphi_0=1_I$, are the unit [commutative diagrams](../../../../../../commutative-diagram.md)

$$
\begin{array}{ccc}
I\bullet X&\xrightarrow{\varphi_{I,X}}&I\diamond X\\
\lambda^\bullet_X\searrow&&\swarrow\lambda^\diamond_X\\
&X&
\end{array}
\qquad
\begin{array}{ccc}
X\bullet I&\xrightarrow{\varphi_{X,I}}&X\diamond I\\
\rho^\bullet_X\searrow&&\swarrow\rho^\diamond_X\\
&X&.
\end{array}
$$

Together with the assumed [naturality](../../../../../../naturality.md), these are exactly the axioms for the requested monoidal structure. **There are no further coherence conditions.**

The faithful [strict monoidal functor](../../../../../../strict-monoidal-functor.md) $U$ allows all three diagrams to be checked after applying it. Both tensor structures then have the same underlying tensor and constraints in $\mathcal V$. In particular, the unit conditions are equivalent to

$$
\boxed{U\varphi_{I,X}=1_{UI\otimes UX},\qquad U\varphi_{X,I}=1_{UX\otimes UI}.}
$$

The associativity square becomes the displayed diagram with every tensor replaced by $\otimes$, both associators by $\alpha^{\mathcal V}$, and every $\varphi$ by $U\varphi$. Faithfulness reflects equality of the two resulting composites. One should not identify $\varphi_{I,X}$ itself with an identity in $\mathcal C$: its domain and codomain can be distinct objects with the same image under $U$. Intrinsically it is $(\lambda^\diamond_X)^{-1}\lambda^\bullet_X$, and similarly on the right.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

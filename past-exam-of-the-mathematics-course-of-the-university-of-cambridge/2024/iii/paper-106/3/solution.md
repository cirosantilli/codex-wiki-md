<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Hahn-Banach separation theorem for two convex sets](../../../../../hahn-banach-separation-theorem-for-two-convex-sets.md) states that if $A$ and $B$ are disjoint nonempty convex subsets of a real [locally convex space](../../../../../locally-convex-space.md) $X$ and $A$ is open, then there are a continuous linear functional $f\in X^*$ and a real number $c$ such that

$$
f(a)<c\leq f(b)
\qquad(a\in A, b\in B).
$$

To prove it, form

$$
C=A-B=\{a-b:a\in A, b\in B\}.
$$

This is open and convex and does not contain zero. The [separation of a point and an open convex set](../../../../../separation-of-a-point-and-an-open-convex-set.md), proved from the [Minkowski functional](../../../../../minkowski-functional.md) and the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md), gives a nonzero continuous $f$ with $f(c)<0$ for every $c\in C$. Hence $f(a)<f(b)$ for all $a,b$. Taking $c$ between $\sup_Af$ and $\inf_Bf$ gives the stated form.

For a [dual pair](../../../../../dual-pair.md) $(E,F)$, the topology $\sigma(E,F)$ has a neighbourhood base at zero consisting of

$$
\{x:|f_j(x)|<\varepsilon, 1\leq j\leq n\},
\qquad f_j\in F.
$$

Every $f\in F$ is continuous by definition. Conversely, if a linear functional $g$ is continuous, some such neighbourhood lies in $\{|g|<1\}$. Therefore $\bigcap_j\ker f_j\subseteq\ker g$. Elementary linear algebra then gives $g\in\operatorname{span}\{f_1,\ldots,f_n\}\subseteq F$. Thus

$$
\boxed{(E,\sigma(E,F))^*=F}.
$$

For a normed space $X$, the weak topology is $\sigma(X,X^*)$; on $X^*$ the weak-star topology is $\sigma(X^*,X)$, using the canonical image of $X$ in $X^{**}$. If $X$ is reflexive, $X^{**}=J_X(X)$, so the weak and weak-star topologies on $X^*$ coincide. Conversely, if they coincide, every $x^{**}\in X^{**}$ is weak-star continuous. The dual-pair result says that every such functional is evaluation at some $x\in X$, so $J_X$ is onto and $X$ is reflexive.

For $A\subseteq E$, every $a\in A$ and zero satisfy every inequality defining $A^{\circ\circ}$, so $A\cup\{0\}\subseteq A^{\circ\circ}$. The latter is an intersection of weakly closed convex half-spaces, hence contains

$$
C=\overline{\operatorname{conv}}^{\sigma(E,F)}(A\cup\{0\}).
$$

If $x\notin C$, choose an open convex neighbourhood $V$ of zero with $(x+V)\cap C=\varnothing$. Applying the separation theorem to $x+V$ and $C$ gives $f\in F$ with

$$
\sup_{c\in C}f(c)<f(x).
$$

Because $0\in C$, the supremum is nonnegative. After multiplying $f$ by a positive scalar, $f\leq1$ on $C$ while $f(x)>1$. Thus $f\in A^\circ$ but $x\notin A^{\circ\circ}$. We conclude with the [Bipolar theorem for a dual pair](../../../../../bipolar-theorem-for-a-dual-pair.md):

$$
\boxed{A^{\circ\circ}=\overline{\operatorname{conv}}^{\sigma(E,F)}(A\cup\{0\}).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

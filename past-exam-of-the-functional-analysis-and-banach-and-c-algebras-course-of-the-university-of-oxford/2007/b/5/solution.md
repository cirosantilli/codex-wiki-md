<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [C-star algebra](../../../../c-star-algebra.md) is a complex [Banach algebra](../../../../banach-algebra-split.md) with a conjugate-linear [involution](../../../../involution.md) satisfying $(ab)^*=b^*a^*$, $(a^*)^*=a$ and $\|a^*a\|=\|a\|^2$. It is unital when it has an identity for multiplication. For $B(H)$ use composition and the Hilbert adjoint. Completeness in the [operator norm](../../../../operator-norm.md) is given; composition is submultiplicative and the adjoint has the required algebraic properties. For a unit vector $\xi$,

$$
\|T\xi\|^2=\langle T^*T\xi,\xi\rangle\leq\|T^*T\|.
$$

Taking the supremum and using the opposite bound $\|T^*T\|\leq\|T^*\|\|T\|=\|T\|^2$ proves the [C-star identity](../../../../c-star-identity.md). Its identity is $I_H$, proving **$B(H)$ is a unital [C-star algebra](../../../../c-star-algebra.md)**.

[Compact operators](../../../../compact-operator-split.md) form a [norm](../../../../norm.md)-closed linear space and are stable under composition with bounded operators. They are also adjoint stable. To see this directly, choose a finite $\varepsilon$-net of the compact image of the [unit ball](../../../../unit-ball.md) under $T$, and let $P$ project orthogonally onto the span of its centers. Then $\|(I-P)T\|\leq\varepsilon$. The [finite-rank operator](../../../../finite-rank-operator.md) $T^*P$ approximates $T^*$ with the same error, so $T^*$ is compact by [norm](../../../../norm.md) closure. Thus **$\mathcal K(H)$ is a [C-star algebra](../../../../c-star-algebra.md)**, with the inherited [norm](../../../../norm.md) and operations.

If it has a multiplicative identity $E$, apply $ER=R$ to every [rank-one operator](../../../../rank-one-operator.md) with arbitrary prescribed range vector $\xi$. Evaluating that equation on a vector sent to $\xi$ gives $E\xi=\xi$. Hence $E=I_H$. This identity is compact exactly when $H$ is finite dimensional: finite dimension gives compactness of the [unit ball](../../../../unit-ball.md), while in infinite dimension an infinite [orthonormal sequence](../../../../orthonormal-sequence.md) has pairwise distance $\sqrt2$ and no convergent subsequence. Therefore **$\mathcal K(H)$ is unital exactly in finite dimension**, with the zero-algebra convention understood if $H=0$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

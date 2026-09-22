<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fix $x$ with $x^N=0$ as a [matrix](../../../../matrix.md). On the full [matrix](../../../../matrix.md) algebra define $L_x(y)=xy$ and $R_x(y)=yx$. These endomorphisms commute and each has $N$th power zero. The [Adjoint representation of a Lie algebra](../../../../adjoint-representation-of-a-lie-algebra.md) is $\operatorname{ad}(x)=L_x-R_x$. The binomial theorem gives

$$
(\operatorname{ad}x)^m(y)=\sum_{j=0}^{m}(-1)^j\binom mjx^{m-j}yx^j.
$$

For $m=2N-1$, each summand has either $j\ge N$ or $m-j\ge N$, and hence vanishes. Therefore $\operatorname{ad}(x)$ is nilpotent on the full [matrix](../../../../matrix.md) algebra and on its [invariant subspace](../../../../invariant-subspace.md) $\mathfrak g$.

[Engel's theorem](../../../../engel-s-theorem.md), in its adjoint form, states that a finite-dimensional [Lie algebra](../../../../lie-algebra-split.md) is nilpotent if every $\operatorname{ad}(x)$ is a [nilpotent endomorphism](../../../../nilpotent-linear-map.md). Applying it to all $x\in\mathfrak g$ proves

$$
\boxed{\mathfrak g\text{ is nilpotent}.}
$$

This is distinct from assuming that an arbitrary [representation](../../../../group-representation.md) of a nilpotent algebra must act by nilpotent matrices, which is false.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Lie algebras course of the University of Oxford](../../../split.md)
5. [Lie algebras course of the University of Oxford](../../../../lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

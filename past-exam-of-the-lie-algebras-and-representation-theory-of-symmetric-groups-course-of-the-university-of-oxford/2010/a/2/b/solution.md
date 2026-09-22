<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The flag makes every [composition factor](../../../../../composition-factor.md) one-dimensional, described by a [character](../../../../../character-of-a-representation.md) $\lambda:H\to F$. The [Jordan–Hölder theorem for modules](../../../../../jordan-holder-theorem-for-modules.md) for finite-length modules says that the multiset of simple composition factors is independent of the chosen composition series.

Here is a construction valid over every $F$. For $h\in H$, every [generalized eigenspace](../../../../../generalized-eigenspace.md) of $\rho(h)$ is an $H$-[submodule](../../../../../submodule.md). Indeed $\operatorname{ad}(h)$ is nilpotent on $H$, say of exponent $c$, and

$$
(\rho(h)-aI)^N\rho(x)
=\sum_{j=0}^N\binom Nj\rho((\operatorname{ad}h)^jx)(\rho(h)-aI)^{N-j}.
$$

If $v$ is killed by $(\rho(h)-aI)^{N_0}$, take $N\ge N_0+c$. Terms with $j\ge c$ vanish by adjoint nilpotence, and all other terms kill $v$. This proves invariance of the [generalized eigenspace](../../../../../generalized-eigenspace.md).

The flag also makes the [characteristic polynomial](../../../../../characteristic-polynomial.md) of every $\rho(h)$ split over $F$. Whenever two composition characters differ, choose an $h$ on which they differ and split the [module](../../../../../module-mathematics.md) into the distinct generalized eigenspaces of $\rho(h)$. Repeat within each summand until all its composition factors have the same [character](../../../../../character-of-a-representation.md). Every nontrivial split lowers dimensions, so the process terminates. Finally combine summands carrying the same [character](../../../../../character-of-a-representation.md). Jordan–Hölder ensures that the resulting distinct blocks have distinct factor types, giving

$$
\boxed{V=\bigoplus_\lambda W_\lambda,\qquad
\text{all composition factors of }W_\lambda\text{ have character }\lambda.}
$$

This recursive method does not assume that a single element separates every [character](../../../../../character-of-a-representation.md), which could fail over a finite [field](../../../../../field.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

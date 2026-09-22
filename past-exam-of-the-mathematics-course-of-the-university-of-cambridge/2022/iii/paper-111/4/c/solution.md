<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Order the chambers $wK$ by nondecreasing [Coxeter length](../../../../../../coxeter-length.md), beginning with $K$. When $wK$ is attached, let

$$
T(w)=\{s\in S:\ell(ws)<\ell(w)\}
$$

be its right descent set. Claim C2 applied to the coset $wW_{T(w)}$, followed by C1, shows that $T(w)$ is spherical. The part of $wK$ already present is exactly

$$
wK^{T(w)}=w\bigcup_{s\in T(w)}K_s.
$$

It is nonempty for $w\ne e$ and is contractible by C3. The chamber $wK$ is contractible as well, so C4 shows inductively that every finite length-ordered union of chambers is contractible.

The Davis complex is a [CW complex](../../../../../../cw-complex.md) and is the increasing union of these chamber unions. Every map from a sphere has compact image and therefore lies in a finite union; the next finite contractible union null-homotopes it. Thus every homotopy group of the Davis complex vanishes. Since it is connected, the [Whitehead theorem](../../../../../../whitehead-theorem.md) implies

$$
\boxed{\Sigma(W,S)\text{ is contractible}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

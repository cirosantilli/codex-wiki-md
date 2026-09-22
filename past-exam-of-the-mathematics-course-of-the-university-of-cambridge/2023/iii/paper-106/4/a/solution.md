<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The useful forms of the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) in a real locally convex space are:

- if $C$ is nonempty open convex and $x\notin C$, there are a continuous linear functional $f$ and $\alpha\in\mathbb R$ with $f(c)<\alpha\leq f(x)$ for every $c\in C$;
- if $C$ is closed convex and $x\notin C$, there are $f$ and $\alpha$ with $\sup_Cf<\alpha<f(x)$;
- if $K$ is compact convex, $C$ is closed convex, and $K\cap C=\varnothing$, there are $f$ and $\alpha<\beta$ with $\sup_Cf<\alpha<\beta<\inf_Kf$, after changing the sign of $f$ if needed.

The [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) says that the closed unit ball of $E^*$ is compact in $\sigma(E^*,E)$. [Goldstine theorem](../../../../../../goldstine-theorem.md) says that the canonical image of the closed unit ball of a normed space $E$ is weak-star dense in the closed unit ball of $E^{**}$.

Give $Z$ its norm inherited from $X^*$ and define

$$
J:X\longrightarrow Z^*,\qquad Jx(f)=f(x).
$$

It is linear and contractive, and it is injective because $Z$ separates points. Goldstine's theorem followed by restriction from $X^*$ to $Z$ shows that $J(B_X)$ is weak-star dense in $B_{Z^*}$: a functional on $Z$ first extends norm-preservingly to $X^*$, and elements of $B_X$ approximate that extension on every finite subset of $Z$.

The topology induced by $\sigma(Z^*,Z)$ on $J(B_X)$ is exactly the given topology $\sigma(X,Z)$. By hypothesis $B_X$ is compact, so $J(B_X)$ is weak-star compact and therefore closed in the Hausdorff space $B_{Z^*}$. Density now gives

$$
J(B_X)=B_{Z^*}.
$$

**Thus $J$ is surjective and maps closed unit ball onto closed unit ball, so it is an isometric isomorphism. Hence $X$ is a dual space. This is the [compact norming dual-pair criterion](../../../../../../compact-norming-dual-pair-criterion.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

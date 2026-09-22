<h1 id="21f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The map $p$ is the quotient of $\mathbb R^2$ by integer translations, and

$$
p^{-1}(x_0)=\mathbb Z^2.
$$

Given a [based loop](../../../../../../based-loop.md) $\gamma$ at $x_0$, the [path lifting theorem](../../../../../../path-lifting-theorem.md) gives a unique lift $\widetilde\gamma$ beginning at $0$. Its endpoint lies in $\mathbb Z^2$. The [homotopy lifting property](../../../../../../homotopy-lifting-property.md) shows that this endpoint depends only on $[\gamma]$, so define

$$
\Phi:\pi_1(X,x_0)\to\mathbb Z^2,
\qquad
\Phi([\gamma])=\widetilde\gamma(1).
$$

Lifting a concatenation after translating the second lift by the endpoint of the first shows that $\Phi$ is a [group homomorphism](../../../../../../group-homomorphism.md). It is surjective because, for every $m\in\mathbb Z^2$, the path $r\mapsto p(rm)$ is a loop whose lift ends at $m$. If a lift ends at zero, it is a loop in the simply connected space $\mathbb R^2$ and contracts there; projecting the contraction proves that its original loop is null-homotopic. Thus $\Phi$ is injective, and the [lift-endpoint description of the fundamental group of the torus](../../../../../../lift-endpoint-description-of-the-fundamental-group-of-the-torus.md) gives

$$
\boxed{\pi_1(X,x_0)\cong\mathbb Z^2}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

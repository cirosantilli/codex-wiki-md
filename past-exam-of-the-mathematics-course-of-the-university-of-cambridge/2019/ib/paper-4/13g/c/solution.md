<h1 id="13g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define a continuous map $F:S\to T$ by the standard [embedded torus of revolution](../../../../../../embedded-torus-of-revolution.md) parametrization

$$
F(s,t)=\bigl((2+\cos2\pi t)\cos2\pi s,
(2+\cos2\pi t)\sin2\pi s,
\sin2\pi t\bigr).
$$

Its image lies in $T$ because

$$
\sqrt{x^2+y^2}=2+\cos2\pi t,
\qquad
(\sqrt{x^2+y^2}-2)^2+z^2=1.
$$

The periodicity of the [trigonometric functions](../../../../../../trigonometric-function.md) makes $F(s,0)=F(s,1)$ and $F(0,t)=F(1,t)$, so $F$ is constant on every $\sim$-equivalence class. The [universal property of the quotient topology](../../../../../../universal-property-of-the-quotient-topology.md) therefore gives a unique continuous map

$$
\overline F:S/{\sim}\longrightarrow T,
\qquad
\overline F([s,t])=F(s,t).
$$

Every point of $T$ has cylindrical radius between $1$ and $3$, so its polar angle determines $s$ modulo one, while the pair $(\sqrt{x^2+y^2}-2,z)$ on the [unit circle](../../../../../../complex-unit-circle.md) determines $t$ modulo one. Hence $\overline F$ is surjective, and two parameters have the same image exactly when they differ by the endpoint identifications defining $\sim$; thus it is injective.

The quotient $S/{\sim}$ is compact as the continuous image of the given compact space $S$ under the [quotient map](../../../../../../quotient-map.md). The surface $T$ is Hausdorff because it has the [subspace topology](../../../../../../subspace-topology.md) inherited from $\mathbb R^3$. The [compact-to-Hausdorff continuous bijection theorem](../../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) now shows that $\overline F$ is a homeomorphism. Therefore

$$
\boxed{S/{\sim}\cong T}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13G](../../13g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

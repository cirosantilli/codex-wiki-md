<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x$ in a unital complex algebra $A$, the [spectrum of an element](../../../../../../spectrum-of-an-element.md) is

$$
\sigma_A(x)=\{\lambda\in\mathbb C:x-\lambda1\text{ is not invertible}\}.
$$

For a nonunital algebra one uses its [unitization](../../../../../../unitization-of-an-algebra.md).

Now let $A$ be a [Banach algebra](../../../../../../banach-algebra-split.md). The invertible group is open, so the [resolvent set](../../../../../../resolvent-of-an-element.md) is open and the spectrum is closed. If $|\lambda|>\lVert x\rVert$, the [Neumann series](../../../../../../neumann-series.md)

$$
(\lambda1-x)^{-1}
=\lambda^{-1}\sum_{n=0}^\infty(x/\lambda)^n
$$

converges, so $\sigma_A(x)$ is contained in the closed disc of radius $\lVert x\rVert$ and is therefore compact.

If the spectrum were empty, $R(\lambda)=(\lambda1-x)^{-1}$ would be an entire $A$-valued function. For each $f\in A^*$, the scalar function $f(R(\lambda))$ is bounded: it tends to zero at infinity by the Neumann series and is bounded on every compact disc. The [Liouville theorem](../../../../../../liouville-theorem.md) makes it identically zero. Since the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) separates points, this would give $R(\lambda)=0$, contradicting its invertibility. Hence the spectrum is nonempty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

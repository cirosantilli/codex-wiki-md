<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the usual irreducible [algebraic variety](../../../../../../algebraic-variety.md) convention here, and write $N=\dim X$, $r=\dim Y$. Fix a closed point $y$ and an affine neighborhood $Y_0$ of it. [Noether normalization](../../../../../../noether-normalization.md) gives a finite surjective map $\pi:Y_0\to\mathbb A^r$. Put $a=\pi(y)$. Its fibre is a finite set $\{y_1,\ldots,y_s\}$, one of whose members is $y$, because a [finite morphism](../../../../../../finite-morphism.md) has finite fibres over closed points.

Choose an affine open $U\subseteq\phi^{-1}(Y_0)$ meeting $X_y$. Since $X$ is irreducible, $U$ still has dimension $N$. In $U$, the fibre of $\pi\phi$ over $a$ is cut out by the $r$ [regular functions](../../../../../../regular-function.md) $\pi_j\phi-a_j$. Apply the supplied [principal hypersurface dimension lemma](../../../../../../principal-hypersurface-dimension-lemma.md) successively on each [irreducible component](../../../../../../irreducible-component.md): if a function vanishes identically the dimension does not drop, if its zero set is empty the component disappears, and otherwise each new component loses exactly one dimension. Hence every surviving component after the $r$ cuts has dimension at least $N-r$.

But that composite fibre is the disjoint union of $U\cap\phi^{-1}(y_i)$. Each member is closed, and since there are finitely many members it is also open in the composite fibre. Thus $U\cap X_y$ is a nonempty union of its [irreducible components](../../../../../../irreducible-component.md), giving

$$
\boxed{\dim X_y\ge\dim(U\cap X_y)\ge N-r=\dim X-\dim Y.}
$$

The same argument around a point on any fibre component gives the componentwise bound. This is the [closed-fibre lower bound by finite normalization](../../../../../../closed-fibre-lower-bound-by-finite-normalization.md); it avoids assuming that $Y$ is smooth or that its point ideal has only $r$ generators.

Irreducibility matters if “variety” is generalized to arbitrary reduced reducible spaces. For example $X=\mathbb A^2\sqcup\mathbb A^1\to\mathbb A^1$ can map the first component constantly to zero and the second by the identity. It is surjective, but nonzero fibres have dimension zero while $\dim X-\dim Y=1$. For reducible sources one uses the individual component dimensions instead; the preceding proof establishes the stated theorem under its standard irreducible-variety convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

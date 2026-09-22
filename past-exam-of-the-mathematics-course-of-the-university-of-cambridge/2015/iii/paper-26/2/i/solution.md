<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $e_1,\ldots,e_d$ be a $\mathbb Q_p$-basis of $K$, and define the coordinate norm

$$
\left\|\sum_j x_je_j\right\|_0=\max_j|x_j|_p.
$$

First an extending [absolute value on a field](../../../../../../absolute-value-algebra.md) is automatically non-Archimedean. Its values on integers are at most one, and the binomial theorem gives

$$
|x+y|^m\leq(m+1)\max(|x|,|y|)^m.
$$

Taking $m$th roots and letting $m\to\infty$ proves the ultrametric inequality.

Consequently

$$
|x|\leq C\|x\|_0,\qquad C=\max_j|e_j|.
$$

This bound makes $x\mapsto|x|$ continuous for the coordinate topology. The coordinate sphere $S=\{x:\|x\|_0=1\}$ is a closed subset of $\mathbb Z_p^d$, hence compact. It contains no zero, so the continuous positive function $|x|$ attains a positive minimum $c$ there. Scaling any nonzero vector by a power of $p$ to put it in $S$ proves

$$
\boxed{c\|x\|_0\leq|x|\leq C\|x\|_0.}
$$

This is the [compact-sphere proof of finite-dimensional non-Archimedean norm equivalence](../../../../../../compact-sphere-proof-of-finite-dimensional-non-archimedean-norm-equivalence.md).

A Cauchy sequence for $|\cdot|$ is therefore Cauchy in each coordinate. The completeness of $\mathbb Q_p$ gives a coordinate limit, and the upper bound gives convergence to it for $|\cdot|$. Thus **every extending absolute value makes $K$ complete**.

For uniqueness, if $|\cdot|_1$ and $|\cdot|_2$ are two extensions, their respective bounds give constants $A,B>0$ with

$$
A|x|_1\leq|x|_2\leq B|x|_1.
$$

Apply this to $x^m$ and use multiplicativity:

$$
A^{1/m}|x|_1\leq|x|_2\leq B^{1/m}|x|_1.
$$

Letting $m\to\infty$ proves $\boxed{|x|_1=|x|_2}$ for every $x$. This proves the [unique extension of an absolute value to a finite extension](../../../../../../unique-extension-of-an-absolute-value-to-a-finite-extension.md) without assuming that an arbitrary coordinate norm is multiplicative.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

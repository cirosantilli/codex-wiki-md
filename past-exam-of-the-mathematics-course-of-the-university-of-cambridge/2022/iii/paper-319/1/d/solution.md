<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $y\in D(A)$, the [semigroup property](../../../../../../semigroup-property.md) gives

$$
\frac{U(h)U(t)y-U(t)y}{h}
=U(t)\frac{U(h)y-y}{h}\longrightarrow U(t)Ay.
$$

Hence $U(t)y\in D(A)$ and

$$
AU(t)y=U(t)Ay.
$$

The [generator domain](../../../../../../generator-domain.md) is therefore an [invariant subspace](../../../../../../invariant-subspace.md), and the [operator norm](../../../../../../operator-norm.md) bound gives

$$
\begin{aligned}
\|\widetilde U(t)y\|_Y
&=\|U(t)y\|+\|AU(t)y\|\\
&=\|U(t)y\|+\|U(t)Ay\|\\
&\leq Me^{\omega t}\bigl(\|y\|+\|Ay\|\bigr).
\end{aligned}
$$

Thus

$$
\boxed{\|\widetilde U(t)y\|_Y\leq Me^{\omega t}\|y\|_Y}.
$$

Moreover, [strong continuity](../../../../../../strong-continuity.md) applied separately to $y$ and $Ay$ gives

$$
\|\widetilde U(t)y-y\|_Y
=\|U(t)y-y\|+\|U(t)Ay-Ay\|\longrightarrow0.
$$

Therefore the restrictions form the [semigroup restricted to its generator domain](../../../../../../semigroup-restricted-to-its-generator-domain.md). Its derivative at zero exists in the [graph norm](../../../../../../graph-norm.md) exactly when $y\in D(A)$ and $Ay\in D(A)$, namely when $y\in D(A^2)$, and then the derivative is $Ay$. Hence its generator is

$$
\boxed{A|_{D(A^2)},\qquad D(A^2)=\{y\in D(A):Ay\in D(A)\}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

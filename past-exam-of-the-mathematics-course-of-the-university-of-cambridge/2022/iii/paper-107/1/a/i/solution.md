<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set

$$
A=\sup_{\partial\Omega}|u|,
\qquad
B=\sup_\Omega|f|,
\qquad
v(x)=A+B(e^{2d}-e^{x_1+d}).
$$

Then $v\geq A$ and, because $1\leq e^{x_1+d}\leq e^{2d}$ and $c\leq0$,

$$
(\Delta+c)v=-Be^{x_1+d}+cv\leq-B.
$$

Thus $(\Delta+c)(u-v)=f-(\Delta+c)v\geq0$ and $u-v\leq0$ on the boundary. The [weak maximum principle for elliptic operators](../../../../../../../weak-maximum-principle-for-elliptic-operators.md) gives $u\leq v$. Applying the same argument to $-u$ gives $|u|\leq v$, hence

$$
\boxed{\sup_\Omega|u|
\leq\sup_{\partial\Omega}|u|
+(e^{2d}-1)\sup_\Omega|f|.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

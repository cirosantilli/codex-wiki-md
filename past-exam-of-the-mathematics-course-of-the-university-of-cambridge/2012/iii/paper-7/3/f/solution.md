<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

We prove [compact perturbation invariance of Fredholm operators](../../../../../../compact-perturbation-invariance-of-fredholm-operators.md) using a two-sided inverse modulo compact operators. If $L$ is [Fredholm](../../../../../../fredholm-operator.md), decompose

$$
H=\ker L\oplus(\ker L)^\perp,\qquad
H=\operatorname{ran}L\oplus(\operatorname{ran}L)^\perp.
$$

The restriction of $L$ from $(\ker L)^\perp$ to its closed range is a bounded bijection, so the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) supplies a bounded inverse there. Extend that inverse by zero on $(\operatorname{ran}L)^\perp$ to obtain a bounded operator $B$. If $P,Q$ are the [orthogonal projections](../../../../../../orthogonal-projection.md) onto $\ker L$ and $(\operatorname{ran}L)^\perp$, respectively, then

$$
BL=I-P,\qquad LB=I-Q.
$$

Both $P$ and $Q$ have finite rank.

Set $T=L+K$. Products of a [compact operator](../../../../../../compact-operator-split.md) and a bounded operator are compact: on one side compactness preserves compact images, and on the other the bounded operator maps the unit ball into a bounded ball. Hence

$$
BT=I+C,\qquad TB=I+D,\qquad
C=-P+BK,\quad D=-Q+KB,
$$

where $C,D$ are compact.

Here is why these identities force $T$ to be [Fredholm](../../../../../../fredholm-operator.md). On $\ker T$, $C=-I$, so part (a) and compactness make $\ker T$ finite-dimensional. There is a positive constant $c$ with

$$
\|Th\|\geq c\|h\|\qquad(h\perp\ker T).
$$

Otherwise unit vectors $h_n\perp\ker T$ could satisfy $Th_n\to0$. From $h_n=-Ch_n+BTh_n$ and compactness, a subsequence would converge strongly to a unit vector $h\perp\ker T$ with $Th=0$, which is impossible. The lower bound proves closed range: for a convergent sequence $Th_n$, first discard the kernel components, then the remaining $h_n$ are Cauchy and their limit maps to the desired range limit.

For finite codimension, take the [adjoint operator](../../../../../../adjoint-operator.md) of $TB=I+D$, giving $B^*T^*=I+D^*$. The operator $D^*$ is compact: the finite-rank approximation proved in part (e) gives finite-rank adjoints converging in [operator norm](../../../../../../operator-norm.md) to $D^*$, and norm limits of compact operators are compact. On $\ker T^*$, $D^*=-I$, so this kernel is finite-dimensional. Finally,

$$
(\operatorname{ran}T)^\perp=\ker T^*.
$$

Because the range is closed, its [cokernel](../../../../../../cokernel.md) is isomorphic to this finite-dimensional orthogonal complement. This verifies all three [Fredholm operator](../../../../../../fredholm-operator.md) conditions for $L+K$.

For the converse, start with $L+K$ and perturb by the compact operator $-K$. **Therefore $L$ is Fredholm if and only if $L+K$ is Fredholm**, with no self-adjointness assumption.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

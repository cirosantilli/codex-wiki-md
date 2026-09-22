<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Identify $\mathbb R^4$ with the [quaternions](../../../../../../quaternion.md), and use the identification of [unit quaternions](../../../../../../unit-quaternion.md) with $SU(2)$ proved in the root Solution. The action

$$
(q_L,q_R):v\longmapsto q_Lvq_R^{-1}
$$

preserves the Euclidean [norm](../../../../../../norm.md) by multiplicativity of [quaternion](../../../../../../quaternion.md) [norms](../../../../../../norm.md). It is a homomorphism $SU(2)\times SU(2)\to SO(4)$: its domain is connected, so the orthogonal image has [determinant](../../../../../../determinant.md) $+1$.

An element in the kernel fixes $v=1$, giving $q_L=q_R=q$. Fixing every other $v$ means $q$ commutes with all [quaternions](../../../../../../quaternion.md), so $q$ is real; since it has unit [norm](../../../../../../norm.md), $q=\pm1$. Hence the kernel is the diagonal subgroup $\{(1,1),(-1,-1)\}$.

The differential acts as $v\mapsto av-vb$ for imaginary [quaternions](../../../../../../quaternion.md) $a,b$. If it vanishes, $v=1$ gives $a=b$, and commutation with all $v$ makes $a$ real and imaginary, hence zero. The differential is injective, and both [Lie algebras](../../../../../../lie-algebra-split.md) have dimension six. The image is therefore an open subgroup of connected $SO(4)$, hence all of $SO(4)$. Thus

$$
\boxed{SO(4)\cong\bigl(SU(2)\times SU(2)\bigr)/\mathbb Z_2,}
$$

where $\mathbb Z_2$ acts diagonally, not separately on the two factors.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The empty-set case is immediate; take $A$ finite and nonempty. Part (ii) gives a nonempty $X\subseteq A$ such that

$$
|X+kA|\le C^k|X|,\qquad |X+lA|\le C^l|X|.
$$

We include the [Ruzsa triangle inequality](../../../../../../ruzsa-triangle-inequality.md) argument to justify passing from sums to differences. For each $d\in kA-lA$, fix one representation $d=u_d-v_d$ with $u_d\in kA$ and $v_d\in lA$. The map

$$
X\times(kA-lA)\longrightarrow(X+kA)\times(X+lA),\qquad
(x,d)\longmapsto(x+u_d,x+v_d)
$$

is injective. Its output difference recovers $d$; the fixed representation then recovers $x$. Hence

$$
|X|\,|kA-lA|\le|X+kA|\,|X+lA|
\le C^{k+l}|X|^2.
$$

Since $|X|\le|A|$, this proves

$$
\boxed{|kA-lA|\le C^{k+l}|A|.}
$$

Only the [abelian group](../../../../../../abelian-group.md) operations were used, so no torsion-free hypothesis is required.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

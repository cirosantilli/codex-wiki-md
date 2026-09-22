<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The map is a homogeneous [Laurent polynomial ring](../../../../../../laurent-polynomial-ring.md) homomorphism between the two rank-one infinity towers. Choose homogeneous generators $e_i$ with absolute degrees $q_i$. Its degree is

$$
\Delta(W,\mathfrak s)=\frac{c_1(\mathfrak s)^2-2\chi(W)-3\sigma(W)}4.
$$

Consequently the general graded-module description is

$$
\boxed{F^\infty_{W,\mathfrak s}(e_1)=a\,U^r e_2,\qquad a\in\mathbb Z,\qquad r=\frac{q_2-q_1-\Delta(W,\mathfrak s)}2.}
$$

If the grading does not allow an integer exponent, the map is zero. Negative exponents are allowed in the infinity theory. The notation $F$ here denotes the map called $\Phi^\infty$ in the question.

The standard topological statements for [Heegaard Floer cobordism maps](../../../../../../heegaard-floer-cobordism-map.md), which require no proof in this part, are

$$
\boxed{b_2^+(W)>0\ \Longrightarrow\ F^\infty_{W,\mathfrak s}=0,\qquad b_2^+(W)=b_1(W)=0\ \Longrightarrow\ F^\infty_{W,\mathfrak s}\text{ is an isomorphism}.}
$$

In the second case $a=\pm1$ and the map is therefore $\pm U^r$ with the exponent determined by the displayed degree formula. Since both boundary components are rational [homology](../../../../../../homology-split.md) [spheres](../../../../../../sphere.md), the rational [intersection form](../../../../../../intersection-form.md) is nondegenerate, so $b_2^+=0$ means that it is negative definite, allowing also the rank-zero form.

The printed hypothesis $b_1(Y_i)=0$ does not imply $b_1(W)=0$. Thus one must not replace the second implication by an unconditional isomorphism assertion for every negative-definite [cobordism](../../../../../../cobordism.md). A concrete check is $W=(S^1\times S^3)\setminus(B^4\sqcup B^4):S^3\to S^3$. It has $b_2^+=0$ and $b_1(W)=1$. A [one-handle](../../../../../../one-handle.md) followed by a [three-handle](../../../../../../three-handle.md) gives $e\mapsto e\otimes\theta^+$ and then kills the $\theta^+$ summand; hence its infinity map is zero. Its grading shift is one, also incompatible with a nonzero map between the even-graded $S^3$ towers. With only the stated boundary assumption, the general homogeneous Laurent-module description and the two topological implications above are the valid conclusions; determining any remaining coefficient requires the actual [cobordism](../../../../../../cobordism.md), not just its boundary Betti numbers.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

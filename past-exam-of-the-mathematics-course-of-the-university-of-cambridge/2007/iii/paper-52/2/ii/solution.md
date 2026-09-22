<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Clebsch-Gordan decomposition for SU2](../../../../../../clebsch-gordan-decomposition-for-su2.md) is

$$
\boxed{V_{j_1}\otimes V_{j_2}\cong\bigoplus_{j=|j_1-j_2|}^{j_1+j_2}V_j,\qquad \dim V_j=2j+1,}
$$

where $j$ increases by one and every summand occurs once. The [tensor product of Lie algebra representations](../../../../../../tensor-product-of-lie-algebra-representations.md) is antihermitian for the product inner product, so an invariant subspace has an invariant orthogonal complement; this gives complete reducibility. To see the particular summands, suppose $j_1\ge j_2$. The product [weight diagram](../../../../../../weight-diagram.md) has one state of weight $j_1+j_2$, two of weight $j_1+j_2-1$, and increasing multiplicities down to the plateau determined by $j_1-j_2$. Subtracting the weight string of $V_{j_1+j_2}$ leaves a single highest state of weight $j_1+j_2-1$. Repeating [highest-weight character subtraction](../../../../../../highest-weight-character-subtraction.md) yields exactly the displayed sequence, down to $j_1-j_2$. Its dimensions exhaust the tensor product because

$$
\sum_{j=j_1-j_2}^{j_1+j_2}(2j+1)=(2j_1+1)(2j_2+1).
$$

The case $j_2\ge j_1$ is identical with the factors exchanged.

Let $C^j_m(m_1,m_2)=\langle m_1:m_2|j,m\rangle$ be the [Clebsch-Gordan coefficients](../../../../../../clebsch-gordan-coefficients.md). Since the total $J_3$ is $J_3^{(1)}\otimes1+1\otimes J_3^{(2)}$, orthogonality of its [eigenspaces](../../../../../../eigenspace.md) gives the selection rule **$C^j_m(m_1,m_2)=0$ unless $m_1+m_2=m$**. Normalize the coupled states by lowering from a unit [highest-weight vector](../../../../../../highest-weight-vector.md), as in part (i); a common phase for an entire summand is immaterial. Then

$$
J_\mp|j,m\rangle=\sqrt{\frac{(j\pm m)(j\mp m+1)}2}|j,m\mp1\rangle.
$$

Take the inner product with $\langle m_1:m_2|$. On the other hand, the total [ladder operator](../../../../../../ladder-operator.md) is $J_\mp^{(1)}\otimes1+1\otimes J_\mp^{(2)}$, and $J_\mp^\dagger=J_\pm$. Its action on the product bra is therefore

$$
\begin{aligned}
\langle m_1:m_2|J_\mp
&=\sqrt{\frac{(j_1\mp m_1)(j_1\pm m_1+1)}2}\langle m_1\pm1:m_2|\\
&\quad+\sqrt{\frac{(j_2\mp m_2)(j_2\pm m_2+1)}2}\langle m_1:m_2\pm1|.
\end{aligned}
$$

Equating the two evaluations and multiplying by $\sqrt2$ proves both signs of the [ladder recurrence for Clebsch-Gordan coefficients](../../../../../../ladder-recurrence-for-clebsch-gordan-coefficients.md):

$$
\boxed{\begin{aligned}
\sqrt{(j\pm m)(j\mp m+1)}\,C^j_{m\mp1}(m_1,m_2)
&=\sqrt{(j_1\mp m_1)(j_1\pm m_1+1)}\,C^j_m(m_1\pm1,m_2)\\
&\quad+\sqrt{(j_2\mp m_2)(j_2\pm m_2+1)}\,C^j_m(m_1,m_2\pm1).
\end{aligned}}
$$

Terms with an index outside its allowed weight range are zero. Merely specifying eigenvectors of $J_3$ would allow unrelated phases for different $m$; the coherent positive-ladder convention above is what makes these recurrences hold with the displayed positive square roots.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

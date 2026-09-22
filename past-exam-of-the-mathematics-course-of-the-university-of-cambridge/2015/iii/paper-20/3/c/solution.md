<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal L=\mathcal O_C(1)$. Its degree is five. Because the linear span of $C$ has dimension at least three, restrictions of linear forms supply at least four independent [global sections](../../../../../../global-section.md), so

$$
h^0(C,\mathcal L)\geq4.
$$

If $h^1(C,\mathcal L)=0$, the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal L)=6-g$, and therefore $g\leq2$ immediately.

If instead $\mathcal L$ is special, the [Clifford inequality for curves](../../../../../../clifford-inequality-for-curves.md) gives

$$
h^0(\mathcal L)\leq1+\frac{\deg\mathcal L}{2}=\frac72,
$$

so its integer dimension is at most three, a contradiction. Here is a short proof of the required [Clifford inequality for curves](../../../../../../clifford-inequality-for-curves.md), so the bound need not be assumed. Put $r=h^0(\mathcal L)>0$ and $s=h^0(\omega_C\otimes\mathcal L^{-1})>0$. At a smooth geometric point, choose bases of these two section spaces with strictly increasing orders of vanishing $a_1<\cdots<a_r$ and $b_1<\cdots<b_s$. Such bases exist because each successive order-of-vanishing quotient has dimension at most one. The products of the first basis with the first element of the second basis, followed by products of the last element of the first basis with the remaining elements of the second, have orders

$$
a_1+b_1<\cdots<a_r+b_1<a_r+b_2<\cdots<a_r+b_s.
$$

They are linearly independent [global sections](../../../../../../global-section.md) of $\omega_C$, proving the [product dimension bound for sections on a curve](../../../../../../product-dimension-bound-for-sections-on-a-curve.md). Thus $r+s-1\leq h^0(\omega_C)=g$. Combining this with [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md), $r-s=\deg\mathcal L+1-g$, gives $2r\leq\deg\mathcal L+2$, which is exactly the displayed [Clifford inequality for curves](../../../../../../clifford-inequality-for-curves.md).

**The special case is impossible, and hence**

$$
\boxed{g(C)\leq2.}
$$

This is the [genus bound for a nonplanar degree-five curve](../../../../../../genus-bound-for-a-nonplanar-degree-five-curve.md). The geometric argument can be carried out after extension to an algebraic closure, which preserves these section dimensions.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

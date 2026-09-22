<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a [basis](../../../../../../basis.md) $\phi_1,\ldots,\phi_N$ of a [conforming finite element space](../../../../../../conforming-finite-element-space.md) $V_N\subset H_0^1(0,1)$ and write $y_N=\sum_jc_j\phi_j$. Testing the [variational problem](../../../../../../variational-problem.md) with each [basis](../../../../../../basis.md) function gives

$$
\boxed{\sum_{j=1}^N A_{ij}c_j=b_i,\qquad
A_{ij}=\int_0^1(\phi_j'\phi_i'+x\phi_j\phi_i)\,dx,\qquad
b_i=\int_0^1f\phi_i\,dx}.
$$

These are also the equations $\partial J(y_N)/\partial c_i=0$ for the [Ritz method](../../../../../../rayleigh-ritz-method.md). The [stiffness matrix](../../../../../../stiffness-matrix.md) is symmetric and a [positive-definite matrix](../../../../../../positive-definite-matrix.md): for a nonzero coefficient [vector](../../../../../../vector.md) $c$, [linear independence](../../../../../../linear-independence.md) gives $v_N=\sum c_j\phi_j\ne0$, and

$$
c^TAc=a(v_N,v_N)\geq\|v_N'\|_{L^2}^2>0.
$$

Thus there is a unique coefficient [vector](../../../../../../vector.md).

Subtracting the exact and discrete [variational problems](../../../../../../variational-problem.md) proves [Galerkin orthogonality](../../../../../../galerkin-orthogonality.md), $a(y-y_N,v_N)=0$ for every $v_N\in V_N$. In the [energy norm](../../../../../../energy-norm.md) $\|v\|_a=\sqrt{a(v,v)}$, the [Pythagorean identity](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) yields

$$
\|y-v_N\|_a^2=\|y-y_N\|_a^2+\|y_N-v_N\|_a^2.
$$

Therefore the [Ritz method](../../../../../../rayleigh-ritz-method.md) is the best approximation in the [energy norm](../../../../../../energy-norm.md). The [Céa lemma](../../../../../../cea-s-lemma.md) also gives $\|y-y_N\|_V\leq(1+\pi^{-2})\inf_{v_N\in V_N}\|y-v_N\|_V$, so any dense sequence of conforming trial spaces converges.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

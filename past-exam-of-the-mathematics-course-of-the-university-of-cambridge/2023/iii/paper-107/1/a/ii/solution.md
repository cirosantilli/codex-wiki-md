<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $0<r<\operatorname{dist}(x,\partial\Omega)$. Differentiating the ball mean-value formula with respect to its centre and then using the [divergence theorem](../../../../../../../divergence-theorem.md) gives

$$
D_i u(x)=\frac1{|B_r|}\int_{B_r(x)}D_i u(y)\,dy
=\frac1{|B_r|}\int_{\partial B_r(x)}u(y)\nu_i(y)\,dS_y.
$$

Consequently the [interior derivative estimate for a harmonic function](../../../../../../../interior-derivative-estimate-for-a-harmonic-function.md) yields

$$
|\nabla u(x)|\leq \frac{C_n}{r}\sup_{B_r(x)}|u|
\leq \frac{C_n}{r}\sup_\Omega|u|.
$$

The constant may depend on $x$ and its distance from the boundary, but it is independent of $u$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

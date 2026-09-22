<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the [vector space](../../../../vector-space-split.md) of nodal values with zero endpoints define the [discrete Sobolev norm](../../../../discrete-sobolev-norm.md)

$$
\boxed{\|W\|_{1,h}=\left(\|W\|_h^2+\|D_x^-W]\!\|_h^2\right)^{1/2}
=\left(h\sum_{i=1}^{N-1}W_i^2+h\sum_{i=1}^N\left(\frac{W_i-W_{i-1}}h\right)^2\right)^{1/2}.}
$$

It is a [norm](../../../../norm.md) because it is the [Euclidean norm](../../../../euclidean-norm.md) of the scaled list of nodal values and first [finite differences](../../../../finite-difference-split.md), and vanishes only for the zero list. It is the discrete counterpart of the [Sobolev space](../../../../sobolev-space-split.md) $H^1$ [norm](../../../../norm.md). Here $W=U-u$ has zero endpoints, so this definition applies directly.

Set $M_4=\max_{0\leq x\leq1}|u^{(4)}(x)|$, finite by the assumed [continuity](../../../../continuous-function.md). [Taylor's theorem](../../../../taylor-s-theorem.md) with fourth-order remainders gives, for suitable $\xi_{i,+}\in(x_i,x_i+h)$ and $\xi_{i,-}\in(x_i-h,x_i)$,

$$
u(x_i\pm h)=u_i\pm hu'_i+\frac{h^2}2u''_i\pm\frac{h^3}6u'''_i+\frac{h^4}{24}u^{(4)}(\xi_{i,\pm}).
$$

Adding the two expansions cancels the odd [derivatives](../../../../derivative.md), so

$$
\varphi_i=\frac{h^2}{24}\left(u^{(4)}(\xi_{i,+})+u^{(4)}(\xi_{i,-})\right),\qquad
|\varphi_i|\leq\frac{M_4h^2}{12}.
$$

Consequently $\|\varphi\|_h^2\leq h(N-1)M_4^2h^4/144\leq M_4^2h^4/144$. Doubling the bound in (c) gives $2\|D_x^-e]\!\|_h^2+\|e\|_h^2\leq\|\varphi\|_h^2$, and therefore

$$
\boxed{\|U-u\|_{1,h}\leq\|\varphi\|_h\leq\frac{M_4}{12}h^2.}
$$

Thus $M_4/12$ is a valid nonnegative constant. To satisfy the request for a strictly positive constant even when $u^{(4)}\equiv0$, take **$C=\max\{1,M_4\}/12$**, independent of $h$. This proves second-order [convergence of a numerical method](../../../../convergence-of-a-numerical-method.md) in a [discrete Sobolev norm](../../../../discrete-sobolev-norm.md), including control of the [backward difference operator](../../../../backward-difference-operator.md) applied to the error.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

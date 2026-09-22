<h1 id="2/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose $T^{(1)}$ and $T^{(2)}$ are two sufficiently regular [steady state](../../../../../../../steady-state.md) solutions with the same prescribed [temperature](../../../../../../../temperature-split.md) on the boundary. Their difference $w=T^{(1)}-T^{(2)}$ satisfies

$$
\nabla\cdot(k\nabla w)=0\quad\hbox{in }R,\qquad w=0\quad\hbox{on }\partial R.
$$

The identical [PDE source terms](../../../../../../../source-term-in-a-partial-differential-equation.md) cancel. Apply the [product rule](../../../../../../../product-rule.md) and the [divergence theorem](../../../../../../../divergence-theorem.md) to $wk\nabla w$; this is the weighted form of [Green's first identity](../../../../../../../green-s-first-identity.md):

$$
\begin{aligned}
0&=\iiint_R w\nabla\cdot(k\nabla w)\,dV\\
&=\iint_{\partial R}wk\nabla w\cdot\mathbf n\,dA-\iiint_Rk\|\nabla w\|^2\,dV
=-\iiint_Rk\|\nabla w\|^2\,dV.
\end{aligned}
$$

Since $k>0$, the nonnegative integrand must vanish, so $\nabla w=0$. Hence $w$ is constant on each connected component of $R$, and its zero [Dirichlet boundary condition](../../../../../../../dirichlet-boundary-condition.md) makes each constant zero. Therefore $\boxed{T^{(1)}=T^{(2)}}$: **the solution, if it exists, is unique**. This proves [Dirichlet uniqueness for variable-conductivity heat conduction](../../../../../../../dirichlet-uniqueness-for-variable-conductivity-heat-conduction.md); it does not require a constant [thermal conductivity](../../../../../../../thermal-conductivity.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Mathematics V](../../../../mathematics-v-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)

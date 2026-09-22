<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The prey have per-capita growth $\mu_1$, loss through encounters with predators at rate $\alpha_1v$, and density-dependent competition $\delta u$. Predators suffer per-capita mortality $\mu_2$, gain from consuming prey at rate $\alpha_2u$, and undergo constant harvesting or removal $\epsilon$. Constant harvesting makes the equations biologically valid only while the predator population remains nonnegative.

At an equilibrium with positive populations,

$$
u=\frac{\mu_1-\alpha_1v}{\delta},\qquad v(\alpha_2u-\mu_2)=\epsilon.
$$

Writing $A=\alpha_2\mu_1-\delta\mu_2>0$ gives

$$
\alpha_1\alpha_2v^2-Av+\delta\epsilon=0,\qquad \boxed{v_\pm=\frac{A\pm\sqrt{A^2-4\alpha_1\alpha_2\delta\epsilon}}{2\alpha_1\alpha_2}.}
$$

For $0<\epsilon<A^2/(4\alpha_1\alpha_2\delta)$, both roots are positive and give $u>\mu_2/\alpha_2>0$ via the second equilibrium equation. Thus there are two positive equilibria.

Using the equilibrium identities in the Jacobian gives

$$
J=\begin{pmatrix}-\delta u&-\alpha_1u\\ \alpha_2v&\epsilon/v\end{pmatrix},\qquad \boxed{\operatorname{tr}J=-\delta u+\frac{\epsilon}{v},\quad \det J=u\left(\alpha_1\alpha_2v-\frac{\delta\epsilon}{v}\right).}
$$

The smaller root satisfies $v_-v_+=\delta\epsilon/(\alpha_1\alpha_2)$ and $v_-<v_+$, so $v_-^2<\delta\epsilon/(\alpha_1\alpha_2)$. Hence its [determinant](../../../../../determinant.md) is negative: **it is always a saddle and unstable**. For small $\delta,\epsilon$, this is the equilibrium with $u\sim\mu_1/\delta$ and $v\sim\delta\epsilon/(\alpha_2\mu_1)$, as required. The [determinant](../../../../../determinant.md) argument is stronger than merely taking the small-parameter limit.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

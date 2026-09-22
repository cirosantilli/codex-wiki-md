<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Along a smooth exact solution, the [chain rule](../../../../../../chain-rule.md) gives $g(y)=f'(y)f(y)=y''$. Expand the unscaled defect of the [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md) about the central time $t_n$. The antisymmetric difference of the solution and second derivative, and the symmetric sum of first derivatives, give

$$
\begin{aligned}
E_h={}&(2-2\alpha-\gamma)h y'+\left(\frac13-\alpha+2\beta\right)h^3y^{(3)}\\
&+\left(\frac1{60}-\frac\alpha{12}+\frac\beta3\right)h^5y^{(5)}+\left(\frac1{2520}-\frac\alpha{360}+\frac\beta{60}\right)h^7y^{(7)}+O(h^9).
\end{aligned}
$$

All derivatives are evaluated at $t_n$. Reflection symmetry removes every even power. The fifth-order conditions require the coefficients of $h,h^3,h^5$ to vanish. The last two equations give $\beta=1/15$ and $\alpha=7/15$, and the first then gives $\gamma=16/15$. Thus

$$
\boxed{\alpha=\frac7{15},\qquad\beta=\frac1{15},\qquad\gamma=\frac{16}{15}.}
$$

These determine the [symmetric two-step two-derivative formula](../../../../../../symmetric-two-step-two-derivative-formula.md). Substitution into the next coefficient gives

$$
E_h=\frac{h^7}{4725}y^{(7)}+O(h^9).
$$

**The requested fifth-order conditions actually produce formal order six.** In the usual maximal-order terminology there is no member of this symmetric family with exact order five: cancelling the fifth-power defect also cancels the automatically zero sixth-power defect. Interpreting the printed request as order at least five gives precisely the boxed parameters.

At zero step size the recurrence polynomial is $w^2-1$, with simple roots $1$ and $-1$, so it satisfies the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) and is [zero-stable](../../../../../../zero-stability.md). With sufficiently smooth locally Lipschitz derivative maps, the nearby implicit solution branch and starting values of matching accuracy, the [convergence of a zero-stable multiderivative method](../../../../../../convergence-of-a-zero-stable-multiderivative-method.md) gives global order six. Formal order by itself does not imply decay of its additional numerical mode.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

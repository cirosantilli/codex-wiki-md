<h1 id="a/2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [boundary layer with exponentially varying outer velocity](../../../../../../boundary-layer-with-exponentially-varying-outer-velocity.md), the ansatz has $u=\Psi_Y=e^{(\beta+\gamma)x}f'(\eta)$. Matching it to $Ae^{\alpha x}$ requires $\beta+\gamma=\alpha$ and $f'(\infty)=A$. The nonlinear terms in the stream-[function](../../../../../../function-split.md) equation scale as $e^{2(\beta+\gamma)x}$, whereas $\Psi_{YYY}$ scales as $e^{(\beta+3\gamma)x}$. Matching exponents gives $\beta=\gamma$, hence

$$
\boxed{\beta=\gamma=\alpha/2.}
$$

More explicitly,

$$
\Psi_Y\Psi_{xY}-\Psi_x\Psi_{YY}
=e^{2\alpha x}\left[\alpha(f')^2-\frac\alpha2ff''\right],\qquad
\Psi_{YYY}=e^{2\alpha x}f''',\qquad U_sU_s'=\alpha A^2e^{2\alpha x}.
$$

Canceling the common factor gives

$$
\boxed{f'''+\frac\alpha2ff''+\alpha\bigl(A^2-(f')^2\bigr)=0.}
$$

Together with $f(0)=0$, the other two conditions are

$$
\boxed{f'(0)=0,\qquad f'(\eta)\longrightarrow A\quad(\eta\to\infty).}
$$

They represent wall no slip and outer-flow matching, respectively.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../../split.md)
7. [Theoretical mechanics course of the University of Oxford](../../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

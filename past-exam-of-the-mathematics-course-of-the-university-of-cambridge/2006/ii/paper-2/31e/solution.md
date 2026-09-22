<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

Orient the circle counterclockwise and define its [Cauchy transform](../../../../../cauchy-transform.md)

$$
\Phi(z)=\frac1{2\pi i}\int_C\frac{\phi(\tau)}{\tau-z}\,d\tau.
$$

The inside and outside limits satisfy $\Phi_+-\Phi_-=\phi$ and $\Phi_++\Phi_-=(\pi i)^{-1}\operatorname{PV}\int_C\phi(\tau)/(\tau-t)\,d\tau$. Also $\Phi_-(z)=O(z^{-1})$ at infinity. Applying these formulas to the two [polynomial](../../../../../polynomial-split.md) coefficients and dividing by $t^2$ gives the Riemann–Hilbert condition

$$
\boxed{(t^2-1)\Phi_+(t)-t\Phi_-(t)=(A-1)t+1.}
$$

The homogeneous jump is $G=t/(t^2-1)$. A [canonical factorization of a rational scalar Riemann-Hilbert jump](../../../../../canonical-factorization-of-a-rational-scalar-riemann-hilbert-jump.md) is

$$
\boxed{X_+(z)=1,\qquad X_-(z)=z-z^{-1},\qquad G=X_+/X_-.}
$$

The inside factor is analytic and nonvanishing; the exterior factor has no zeros or poles outside the circle and grows like $z$. The jump index is $1-2=-1$, consistently with this growth.

Put $F_+=\Phi_+$ and $F_-=\Phi_-/X_-$. Their additive jump is $R(t)=((A-1)t+1)/(t^2-1)$. Since $R$ is analytic outside the circle and decays there, the functions $F_+$ inside and $F_-+R$ outside glue to an [entire function](../../../../../entire-function.md). This function tends to zero at infinity, so [Liouville's theorem](../../../../../liouville-theorem.md) gives $F_+=0$, $F_-=-R$. Consequently

$$
\Phi_+=0,\qquad \Phi_-=-\frac{(A-1)z+1}{z}.
$$

The required decay of a [Cauchy transform](../../../../../cauchy-transform.md) forces **$A=1$**. Then $\Phi_-=-1/z$, and the jump gives

$$
\boxed{\phi(t)=1/t.}
$$

For the homogeneous problem, $\Phi_+/X_+$ and $\Phi_-/X_-$ glue to an [entire function](../../../../../entire-function.md) vanishing at infinity, so only the zero solution exists; this proves uniqueness. Direct verification uses the principal-value integral $-\pi i/t$: the two terms on the left combine to $(t^4+t^3-t^2-t^4+t^3+t^2)/(2t)=t^2$, exactly the right side at $A=1$.

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

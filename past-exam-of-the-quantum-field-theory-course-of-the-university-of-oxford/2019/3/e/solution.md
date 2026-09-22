<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A continuous [Lorentz transformation](../../../../lorentz-transformation.md) in one spatial dimension must preserve $t^2-x^2$. In the component connected to the identity, take the image of the time axis to have velocity $v$, with $|v|<1$, and write $B_v(1,0)^{\mathsf T}=\gamma(1,v)^{\mathsf T}$. Preservation of the [Minkowski norm](../../../../minkowski-norm.md) gives $\gamma^2(1-v^2)=1$, so $\gamma=(1-v^2)^{-1/2}$. The spacelike column must be orthogonal to the timelike column and have squared [Minkowski norm](../../../../minkowski-norm.md) $-1$; continuity fixes it to $\gamma(v,1)^{\mathsf T}$. Thus

$$
\boxed{x'=B_vx,\qquad
B_v=\frac1{\sqrt{1-v^2}}\begin{pmatrix}1&v\\v&1\end{pmatrix}.}
$$

Here $x=(t,x)^{\mathsf T}$ denotes the coordinate pair. This is the positive off-diagonal convention in the source; describing a passive frame moving at $+v$ instead reverses the sign of $v$.

Define the [rapidity](../../../../rapidity.md) $\alpha=\operatorname{artanh}v$. The [hyperbolic function](../../../../hyperbolic-function.md) identities give

$$
\cosh\alpha=\frac1{\sqrt{1-v^2}},\qquad
\sinh\alpha=\frac v{\sqrt{1-v^2}},\qquad
\boxed{B(\alpha)=\begin{pmatrix}\cosh\alpha&\sinh\alpha\\\sinh\alpha&\cosh\alpha\end{pmatrix}.}
$$

In [light-cone coordinates](../../../../light-cone-coordinates.md), $t'+x'=e^\alpha(t+x)$ and $t'-x'=e^{-\alpha}(t-x)$. Therefore the derivatives transform oppositely:

$$
\partial_{t'}+\partial_{x'}=e^{-\alpha}(\partial_t+\partial_x),\qquad
\partial_{t'}-\partial_{x'}=e^{\alpha}(\partial_t-\partial_x).
$$

Use the field-transformation convention $\psi'(x')=S(\alpha)\psi(x)$. The component [action](../../../../action.md) in [c](../c.md) is invariant under

$$
\boxed{\psi_R'(x')=e^{\alpha/2}\psi_R(x),\qquad
\psi_L'(x')=e^{-\alpha/2}\psi_L(x),\qquad
\Lambda_R(\alpha)=e^{\alpha/2},\quad\Lambda_L(\alpha)=e^{-\alpha/2}.}
$$

Indeed, the right-component [kinetic term](../../../../kinetic-term.md) gains $e^{\alpha/2}e^{-\alpha}e^{\alpha/2}=1$, and the left-component [kinetic term](../../../../kinetic-term.md) gains $e^{-\alpha/2}e^{\alpha}e^{-\alpha/2}=1$. The two factors in each [Dirac mass term](../../../../dirac-mass-term.md) cancel as well. Finally $\det B=1$, so $dt'\,dx'=dt\,dx$ and the whole [action](../../../../action.md) is unchanged. These are the [chiral boost weights in two spacetime dimensions](../../../../chiral-boost-weights-in-two-spacetime-dimensions.md).

In [spinor](../../../../spinor.md) notation, $S(\alpha)=\exp(\alpha\gamma^5/2)$ satisfies $S^{-1}\gamma^\mu S=B^\mu{}_{\nu}\gamma^\nu$ and $S^\dagger\gamma^0S=\gamma^0$, so $\bar\psi'=\bar\psi S^{-1}$. These identities directly verify covariance of the [Dirac equation](../../../../dirac-equation.md) and the [Lorentz invariance](../../../../lorentz-invariance.md) of its [action](../../../../action.md). The matrices $S$ are not unitary with respect to the ordinary component norm; the [Dirac adjoint](../../../../dirac-adjoint.md) supplies the invariant bilinear.

The statement about there being only [Lorentz boosts](../../../../lorentz-boost.md) applies to the identity component of the [One-dimensional Lorentz group](../../../../one-dimensional-lorentz-group.md). The full [Lorentz group](../../../../lorentz-group.md) also has discrete transformations: the concrete [spatial reflection](../../../../spatial-reflection.md) $\operatorname{diag}(1,-1)$ preserves the [Minkowski metric](../../../../minkowski-metric.md) but has [determinant](../../../../determinant.md) $-1$, so it cannot equal any displayed $B(\alpha)$, whose [determinant](../../../../determinant.md) is $+1$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [position operators](../../../../../position-operator.md) and [momentum operators](../../../../../momentum-operator.md) are [self-adjoint operators](../../../../../self-adjoint-operator.md). Using conjugate linearity of the [adjoint operator](../../../../../adjoint-operator.md), $(cA+dB)^*=\overline cA^*+\overline dB^*$, gives

$$
\boxed{a_j^*=\frac{m\omega X_j-iP_j}{\sqrt{2m\omega\hbar}}.}
$$

Write $D=\sqrt{2m\omega\hbar}$. Bilinearity and antisymmetry of the [commutator](../../../../../commutator.md), together with the [canonical commutation relations](../../../../../canonical-commutation-relation.md), give $[P_j,X_k]=-i\hbar\delta_{jk}I$. Hence

$$
\begin{aligned}
D^2[a_j,a_k]&=im\omega[X_j,P_k]+im\omega[P_j,X_k]\\
&=-m\omega\hbar\delta_{jk}I+m\omega\hbar\delta_{jk}I=0,\\
D^2[a_j,a_k^*]&=-im\omega[X_j,P_k]+im\omega[P_j,X_k]\\
&=2m\omega\hbar\delta_{jk}I.
\end{aligned}
$$

The terms involving two [position operators](../../../../../position-operator.md) or two [momentum operators](../../../../../momentum-operator.md) vanish by the [canonical commutation relations](../../../../../canonical-commutation-relation.md). Finally, reversing products under the [adjoint operator](../../../../../adjoint-operator.md), $(AB)^*=B^*A^*$, gives $[a_j,a_k]^*=-[a_j^*,a_k^*]$. Therefore

$$
\boxed{[a_j,a_k]=[a_j^*,a_k^*]=0,\qquad [a_j,a_k^*]=\delta_{jk}I.}
$$

Here $I$ is the [identity operator](../../../../../identity-operator.md). These are the relations for two independent pairs of [creation and annihilation operators](../../../../../creation-and-annihilation-operators.md). The [operator algebra](../../../../../operator-algebra.md) in this question is understood on a common invariant [operator domain](../../../../../operator-domain.md), such as finite [linear combinations](../../../../../linear-combination.md) of the [number states](../../../../../number-state.md) constructed in part (c).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
